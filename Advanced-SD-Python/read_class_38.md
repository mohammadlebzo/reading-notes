# Read: Class 38

## Thinking in React

In order to think in React you need to go though a couple of steps, and assuming that you as a developer have a design mock and some JSON data you need to do the following:

### #1 Break The UI Into A Component Hierarchy:

During this stage you need to find your components and look for their connections, and the best way to find that is to think of the single responsibility principle, where each component should be handling one thing only, then you start to look if this component is dependent on another to complete it's job.

### #2 Build A Static Version in React:

During this stage you will be trying to just build the components and make them work as intended, ad because you are building a static version remember, don't use state at all, as this version isn't supposed to be interactive.

### #3 Identify The Minimal (but complete) Representation Of UI State:

During this stage you need to start making the UI interactive using states, and to do that think of the minimal set of mutable state that your actually app needs.

### #4 Identify Where Your State Should Live:

In order to do this you need to think of a couple of things:

- Where does the state make sense.
- does it need direct access to another state higher in the hierarchy.
- the last option if the state home isn't identified you need to build a new component to solely hold it.

## Some more info about React

### Conditional Rendering:

**Conditional rendering** in **React** works just the same as any other programming language, where there is a conditional operator and a condition, and if the condition is met the code will be executed, and in this situation it will be rendered.

ex: ([source](https://reactjs.org/docs/conditional-rendering.html#:~:text=class%20LoginControl%20extends,%3B%0A%20%20%7D%0A%7D))

    class LoginControl extends React.Component {
        constructor(props) {
            super(props);
            this.handleLoginClick = this.handleLoginClick.bind(this);
            this.handleLogoutClick = this.handleLogoutClick.bind(this);
            this.state = {isLoggedIn: false};
        }

        handleLoginClick() {
            this.setState({isLoggedIn: true});
        }

        handleLogoutClick() {
            this.setState({isLoggedIn: false});
        }

        render() {
            const isLoggedIn = this.state.isLoggedIn;
            let button;
            if (isLoggedIn) {
            button = <LogoutButton onClick={this.handleLogoutClick} />;
            } else {
            button = <LoginButton onClick={this.handleLoginClick} />;
            }

            return (
            <div>
                <Greeting isLoggedIn={isLoggedIn} />
                {button}
            </div>
            );
        }
    }

### Lists and Keys:

In order to render an array/list of elements, the array method `map()` is used:

ex: ([source](https://reactjs.org/docs/lists-and-keys.html#:~:text=%3C/li%3E-,%3B,-Then%2C%20we%20can))

    const numbers = [1, 2, 3, 4, 5];
    const listItems = numbers.map((number) =>
    <li>{number}</li>
    );

But React needs a key reference for each one of the elments, so thats why we need to add a key to each element:

ex: ([source](https://reactjs.org/docs/lists-and-keys.html#:~:text=missing%20key%20issue.-,function%20NumberList(props)%20%7B%0A%20%20const%20numbers%20%3D%20props.,ul%3E%7BlistItems%7D%3C/ul%3E%0A%20%20))

    function NumberList(props) {
        const numbers = props.numbers;
        const listItems = numbers.map((number) =>
            <li key={number.toString()}>
            {number}
            </li>
        );
        return (
            <ul>{listItems}</ul>
        );
    }

### Forms:

Forms in React are the same as HTML, but the only difference is that React can use stats to control the form and send data.

ex: ([source](https://reactjs.org/docs/forms.html#:~:text=class%20NameForm%20extends,%3B%0A%20%20%7D%0A%7D))

    class NameForm extends React.Component {
        constructor(props) {
            super(props);
            this.state = {value: ''};

            this.handleChange = this.handleChange.bind(this);
            this.handleSubmit = this.handleSubmit.bind(this);
        }

        handleChange(event) {
            this.setState({value: event.target.value});
        }

        handleSubmit(event) {
            alert('A name was submitted: ' + this.state.value);
            event.preventDefault();
        }

        render() {
            return (
            <form onSubmit={this.handleSubmit}>
                <label>
                Name:
                <input type="text" value={this.state.value} onChange={this.handleChange} />
                </label>
                <input type="submit" value="Submit" />
            </form>
            );
        }
    }

## Things I want to know more about

- None.