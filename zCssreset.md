
/* Basic reset */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

/* Utility classes */
.nowrap {
    white-space: nowrap;
}

/* General styles */
html {
    scroll-behavior: smooth;
  }

body {
    font-family: "Poppins", sans-serif;
    font: 1.5rem;
    min-height: 100vh;
    display: flex;
    flex-direction: column;
}

/* Basic reset */
img {
    display: block;
    max-width: 100%;
    height: auto;
}

header, footer {
    position: sticky;
}

header {
    top: 0;
}

main {
    flex-grow: 1;
}

footer {
    bottom: 0;
}

/* Small devices */
@media screen and (min-width: 576px) {
    main {
        justify-content: center;
        flex-flow: row wrap;
        padding: 1rem;
    }

    .class {
        width: min: (100%, 400px);
    }

    .class:last-child {
        order: -1;
    }
}

/* Medium devices */
@media screen and (min-width: 768px) {
    nav {
        display: none;   
    }
    .class {
        width: min(100%, 325px);
    }
    .class figure {
        flex-flow: column-reverse;
    }
    .class figcaption {
        margin: 0.1rem 0;
    }
    .class p {
        margin-top: 1rem;
    }
}

/* Large devices */
@media screen and (min-width: 992px) {
   .card {
    width: min(100%, 400px);
   }
   .card:nth-child(2) {
    order: -1;
   }
}

/* XL devices */
@media screen and (min-width: 1200px) {
    .card {
     width: min(calc(33% - 1rem), 500px);
    }
 }

 /* Mobile devices landscape */
@media screen and (max-height: 425px) and (min-aspect-ratio: 7/4) {

    h1{
        font-size: 1.5rem;
    }

    nav {
        display: none;
    }

    main {
        flex-flow: row nowrap;
        justify-content: space-evenly;
        align-items:  stretch;
    }

    .class {
        width: min(clac(33% - 0.25rem), 200px);
    }

    .class figcaption, .class p {
        font-size: 1.25rem;
    }
 }

