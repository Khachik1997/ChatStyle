# ChatStyle
Help fixing bug in tailwind css layout
Because Tailwind doesn't hace a calc function to calculate the height of elements I used CSS class.
In the calc function, I should minus all heights from full-screen height and leave only scrollable content height.That's why I write
height: calc(100vh -73px - 65px -50px - 60px - 6rem -2rem - 1rem);
Where`
73px - header height,
65px - nav element height,
50px - chat header height,
60px - input height, then all paddings.
In your project, you can use Javascript to calculate all elements' heights via classes to not confuse pixels by using 
let element = document.getElementById("yourElementId");
let height = element.offsetHeight;

In the code, I left a comment you can uncomment and see more messages and scroll ))
