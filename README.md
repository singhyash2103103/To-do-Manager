To begin:
npx create-react-app my-app
cd my-app
npm start

Delete all default mark up.

For components create folder #components in #src folder and place there your react components. In my project you can see: Form.jsx, FormInput.jsx, List.jsx. You can create as many components as you want and name it how you like.

In this project Material-UI is used. To install run:
npm install @material-ui/core

Material-UI was developed based on the Roboto font. The Roboto font will not be automatically loaded into Material-UI. So be sure to install it.

To install run:
npm install fontsource-roboto

Then import it in "index.js". To do so write in "index.js":
import 'fontsource-roboto';

To use icons run:
npm install @material-ui/icons

Button example:

import  React from 'react';
import Button from "@material-ui/core/Button";

// custom styles with Material UI
const useStyles = makeStyles({
    root: {
        background: 'linear-gradient(45deg, gray 30%, black 90%)',
        border: 0,
        color: 'white',
        height: 30,
        padding: '0 10px',
        whiteSpace: 'nowrap',
        margin: '15px 0 0 20px',
    }
});


const Button = () => {
   const classes = useStyles();
    
   return (
      <Button
           type="submit"
           alt="add-note"
           className={classes.root}
       >
           Add task
       </Button>
     )
     
export  default Button;
Then you can see the result - button "ADD TASK" look like:

Button example

That was easy, right :)
