# Read: Class 37

## React

React is a free and open-source front-end JavaScript library for building user interfaces based on UI components. ([source](https://en.wikipedia.org/wiki/React_(JavaScript_library)#:~:text=React%20(also%20known%20as%20React.js%20or%20ReactJS)%20is%20a%20free%20and%20open%2Dsource%20front%2Dend%20JavaScript%20library%5B3%5D%20for%20building%20user%20interfaces%20based%20on%20UI%20components.))

### Introducing JSX

**JSX** is a syntax extension to JavaScript, used within **React** to describe how the UI should look like.

**JSX** allows users to embed expressions within markup language. ex:

    const name = 'Mike';
    const element = <h1>Hello, {name}</h1>;

The main reason behind using **JSX** is to combine using markup language and Javascript.

### Some things that React allows us to do:

- **Rendering Elements into DOM**. ex: ([source](https://reactjs.org/docs/rendering-elements.html#:~:text=const%20root%20%3D%20ReactDOM.createRoot(%0A%20%20document.getElementById(%27root%27)%0A)%3B%0Aconst%20element%20%3D%20%3Ch1%3EHello%2C%20world%3C/h1%3E%3B%0Aroot.render(element)%3B))

        const root = ReactDOM.createRoot(
            document.getElementById('root')
        );
        const element = <h1>Hello, world</h1>;
        root.render(element);

- **Creating components and props**. ex: ([source](https://reactjs.org/docs/components-and-props.html#:~:text=a%20JavaScript%20function%3A-,function%20Welcome(props)%20%7B%0A%20%20return%20%3Ch1%3EHello%2C%20%7Bprops.name%7D%3C/h1%3E%3B%0A%7D,-This%20function%20is))

        function Welcome(props) {
            return <h1>Hello, {props.name}</h1>;
        }

        class Welcome extends React.Component {
            render() {
                return <h1>Hello, {this.props.name}</h1>;
            }
        }

- **Define everchaging states**. ex: ([source](https://reactjs.org/docs/state-and-lifecycle.html#:~:text=this.state%3A-,class%20Clock%20extends%20React.Component%20%7B%0A%20%20constructor(props),.%3C/h2%3E%0A%20%20%20%20%20%20%3C/div%3E%0A%20%20%20%20)%3B%0A%20%20%7D%0A%7D,-Note%20how%20we)) 

        class Clock extends React.Component {
            constructor(props) {
                super(props);
                this.state = {date: new Date()};
            }

            render() {
                return (
                <div>
                    <h1>Hello, world!</h1>
                    <h2>It is {this.state.date.toLocaleTimeString()}.</h2>
                </div>
                );
            }
        }

## Next.js

Next.js is an open-source web framework that builts on top of Node.js, for the sole reason of allowing React web applications to do the followig:
- Server-side rendering.
- Generating static websites.



## Things I want to know more about

- None.