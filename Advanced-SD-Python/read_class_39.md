# Read: Class 39

## Next.js: Assets, Metadata, and CSS

### Assets:

Next.js provides the users a `public` directory, which is used to store static assets. As for an example of it's offerings:

- **Image Component**:

This component (`next/image`) is an extension of the `<img>` HTML tag, and by using it Next.js would optimize images on-demand, which means that it would not affect building times, and that happens by lazy loading images by default.

Some other benefits of using this component:

- Responsive image for different screen sizes.
- No need for third-party tool for image optimization.

ex: ([source](https://nextjs.org/learn/basics/assets-metadata-css/assets#:~:text=import%20Image%20from%20%27next/image%27%3B%0A%0Aconst%20YourComponent%20%3D%20()%20%3D%3E%20(%0A%20%20%3CImage%0A%20%20%20%20src%3D%22/images/profile.jpg%22%20//%20Route%20of%20the%20image%20file%0A%20%20%20%20height%3D%7B144%7D%20//%20Desired%20size%20with%20correct%20aspect%20ratio%0A%20%20%20%20width%3D%7B144%7D%20//%20Desired%20size%20with%20correct%20aspect%20ratio%0A%20%20%20%20alt%3D%22Your%20Name%22%0A%20%20/%3E%0A)%3B))

    import Image from 'next/image';

    const YourComponent = () => (
        <Image
            src="/images/profile.jpg" // Route of the image file
            height={144} // Desired size with correct aspect ratio
            width={144} // Desired size with correct aspect ratio
            alt="Your Name"
        />
    );

### Metadata:

Next.js Offers a `next/head`, which is used to help in handling metadata, and other info about your application.

### CSS Styling:

Next.js provides some standard styling that are quite helpful, but if you would need to change or add anything, you can:
- Use **Sass**, as Next.js allows `.css` and `.scss` files.
- Use *PostCSS libraries* like **Tailwind** CSS.
- **CSS-in-JS** libraries such as *styled-jsx*, *styled-components*, and *emotion*.

## React context

It is a method od passing and using any kind of data without using props.

**When should you use React context?**

It is useful when the passed data is going to be used by any component in the application. Some examples on these kinds of data whould be: ([source](https://www.freecodecamp.org/news/react-context-for-beginners/#:~:text=These%20types%20of,language%20or%20locale))
- **Theme data**( *dark/white mode*) 
- **Authenticated user data**
- **Location specific data**

### How to use React context?

1. Add `createContext` method within the component you want to use it in.
2. Wrap the context provider around the component tree.
3. Put the values you want to share in the context provider using the `value` prop.
4. Use this value within any component using the context consumer.

ex: ([source](https://www.freecodecamp.org/news/react-context-for-beginners/#:~:text=import%20React%20from%20%27react,Consumer%3E%0A%20%20))

    import React from 'react';

    export const UserContext = React.createContext();

    export default function App() {
        return (
            <UserContext.Provider value="Reed">
            <User />
            </UserContext.Provider>
        )
    }

    function User() {
        return (
            <UserContext.Consumer>
            {value => <h1>{value}</h1>} 
            {/* prints: Reed */}
            </UserContext.Consumer>
        )
    }

## Things I want to know more about

- None.