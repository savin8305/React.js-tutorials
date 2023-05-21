  ## What is CDN 
  `A CDN (Content Delivery Network) in React JS is a system of servers that are distributed around the globe to provide fast delivery of static assets, such as HTML, CSS, JavaScript, and media files, to users. When you use a CDN to serve your React app, the server closest to the user will be used to deliver the content, which helps reduce latency and improve performance. Additionally, some popular CDNs for hosting React applications include Cloudflare, Netlify, GitHub Pages, and AWS S3.`
## What is crossorigin in react CDN
`When using a CDN to serve your React application's scripts, you may need to set the crossorigin attribute to ensure that the browser sends the appropriate headers when fetching the scripts from the CDN.`
## What is createElement("h1",{},"Namaste everyone") explain
`createElement("h1", {}, "Namaste everyone") is a function call in JavaScript that creates an HTML element with the tag h1, sets its attributes to an empty object {}, and sets its inner text to "Namaste everyone".In this case, the h1 element represents a heading level 1 in HTML, and its inner text of "Namaste everyone" would be displayed on the web page as large and bold text. The empty object {} in the second argument could be used to add additional attributes to the h1 element, such as class or id.`




```<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <script src="https://unpkg.com/react@17/umd/react.development.js" crossorigin></script>
    <script src="https://unpkg.com/react-dom@17/umd/react-dom.development.js" crossorigin></script>
    <script src="https://unpkg.com/babel-standalone@6/babel.min.js"></script>
    <title>Document</title>
</head>
<body>
    <div id="root"></div>
</body>
<script type="text/babel">
    // let ele = document.createElement('h1');
    // ele.innerHTML = 'HELLO'
    // let root = document.getElementById('root');
    // console.log(ele)
    // root.appendChild(ele);

    // let ele = React.createElement('h1',{
    //     children:['HELLO']
    // })

    // console.log(ele);
    // root.appendChild(ele);
    // ReactDOM.render(ele,root);

    //JSX

    //Funtional Component
    function Element({name='default',place='idk'}){
        console.log(name)
        return(
            <div>
            <h1>Hello {name}</h1>
            <h6>{place}</h6>
        </div>
        )
    }

    function Main(){
        return(
            <React.Fragment>
                <Element name='Udai' place='delhi'/>
                <Element/>
                <Element/>
                <Element/>
                <Element/>
            </React.Fragment>
        )
    }

    ReactDOM.render(<Main/>,document.getElementById('root'))
</script>
</html>
