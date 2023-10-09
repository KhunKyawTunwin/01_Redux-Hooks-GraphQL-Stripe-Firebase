# Redux-Hooks-GraphQL-Stripe-Firebase

## https://github.com/KhunKyawTunwin/Redux-Hooks-GraphQL-Stripe-Firebase.git

## upgrade React 18

# npm upgrade react rect-dom --latest

## NPM vs YARN

### Throughout the course we will be using Yarn, however using NPM or Yarn is a personal choice. You can use this as a reference guide for the two different commands you can use. Don't worry if you are not sure of the below commands as we will explore them throughout the course:

### Install dependencies from package.json: npm install == yarn

### Install a package and add to package.json: npm install package --save == yarn add package

### Install a devDependency to package.json: npm install package --save-dev == yarn add package --dev

### Remove a dependency from package.json: npm uninstall package --save == yarn remove package

### Upgrade a package to its latest version: npm update --save == yarn upgrade

### Install a package globally: npm install package -g == yarn global add package

## Class Components

## Lifecycle of Components

### Each component in React has a lifecycle which you can monitor and manipulate during its three main phases. The three phases are: Mounting, Updating, and Unmounting.

## Mounting - Mounting means putting elements into the DOM.

### React has four built-in methods that gets called, in this order, whrn mounting a component : 1. contructor() 2. getDerivedStateFromProps() 3. render() 4. componentDidMount()

### The render() method is required and will always be called, the others are optional and will be called if you define them.

## 1. Contructor()

### The constructor() method is called before anything else, when the component is initiated, and it is the natural place to set up the initial state and other initial values. The constructor() method is called with the props, as arguments, and you should always start by calling the super(props) before anything else, this will initiate the parent's constructor method and allows the component to inherit methods from its parent (React.Component).

### class Header extends React.Component {

### constructor(props) {

### super(props);

### this.state = {favoritecolor: "red"};

### }

### render() {

### return (

### <h1>My Favorite Color is {this.state.favoritecolor}</h1>

### );

### }

### }

### const root = ReactDOM.createRoot(document.### getElementById('root'));

### root.render(<Header />);

## Updating

### The next phase in the lifecycle is when a component is updated.

### A component is updated whenever there is a change in the component's state or props.

### React has five built-in methods that gets called, in this order, when a component is updated:

### 1. getDerivedStateFromProps()

### 2. shouldComponentUpdate()

### 3. render()

### 4. getSnapshotBeforeUpdate()

### 5. componentDidUpdate()

### The render() method is required and will always be called, the others are optional and will be called if you define them.
