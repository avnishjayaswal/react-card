Card is container based user interface use HTML for markup and CSS for styling.

<a href="https://askavy.com/react-card/">React Card</a> consist of various elements like header footer images multimedia action and buttons. one can construct different card as per requirement like business card, product card, Ad card, etc

<h1>React Bootstrap Card</h1>

React Bootstrap card are component, Component return a card that built from HTML and bootstrap CSS.

<h2>How to create React Card using bootstrap CSS</h2>

First one need to create a react app

```javascript

npx create-react-app reactcard

```

After that one need to install bootstrap using following command

```javascript

npm install react-bootstrap bootstrap

```

one need to import card component and bootstrap css in App.js

```javascript

import React from 'react';
import 'bootstrap/dist/css/bootstrap.min.css';
import { Card, Button } from 'react-bootstrap';




function App() {
  return (
    <Card style={{ width: '18rem' }}>
      <Card.Img variant="top" src="https://source.unsplash.com/user/erondu/600x400" />
      <Card.Body>
        <Card.Title>Card Title</Card.Title>
        <Card.Text>
          Some Custom text one can write here
        </Card.Text>
        <Button variant="primary">Go somewhere</Button>
      </Card.Body>
    </Card>
  );
}

export default App;


```

Output looks like

<img loading="lazy" width="463" height="599" src="http://askavy.com/wp-content/uploads/2020/07/card-demo.jpg" alt="" class="wp-image-309" srcset="https://askavy.com/wp-content/uploads/2020/07/card-demo.jpg 463w, https://askavy.com/wp-content/uploads/2020/07/card-demo-232x300.jpg 232w" sizes="(max-width: 463px) 100vw, 463px">

<h2>React-bootstrap card image left (Example)</h2>

```javascript

import React from "react";
import "bootstrap/dist/css/bootstrap.min.css";

function App() {
  return (
    <div className="card mb-3" style={{width: '500px'}}>
      <div className="row no-gutters">
        <div className="col-md-4">
          <svg
            className="bd-placeholder-img"
            width="100%"
            height="250"
            xmlns="http://www.w3.org/2000/svg"
            aria-label="Placeholder: Image"
            preserveAspectRatio="xMidYMid slice"
            role="img"
          >
            <title>Placeholder</title>
            <rect width="100%" height="100%" fill="#868e96" />
            <text x="50%" y="50%" fill="#dee2e6" dy=".3em">
              Image
            </text>
          </svg>
        </div>
        <div className="col-md-8">
          <div className="card-body">
            <h5 className="card-title">Card title</h5>
            <p className="card-text">
              Card Text
            </p>
            <p className="card-text">
              <small className="text-muted">Card Text 2</small>
            </p>
          </div>
        </div>
      </div>
    </div>
  );
}

export default App;

```

<h2>Bootstrap card image left
</h2>

<img loading="lazy" width="801" height="431" src="http://askavy.com/wp-content/uploads/2020/08/bootstrap-horizontal-card-with-image.jpg" alt="" class="wp-image-405" srcset="https://askavy.com/wp-content/uploads/2020/08/bootstrap-horizontal-card-with-image.jpg 801w, https://askavy.com/wp-content/uploads/2020/08/bootstrap-horizontal-card-with-image-300x161.jpg 300w, https://askavy.com/wp-content/uploads/2020/08/bootstrap-horizontal-card-with-image-768x413.jpg 768w" sizes="(max-width: 801px) 100vw, 801px">


<h2>Card Columns</h2>

```javascript

import React from "react";
import "bootstrap/dist/css/bootstrap.min.css";
import { Card, CardColumns } from "react-bootstrap";

function CardDisplay() {
  return (
    <CardColumns>
      <Card>
        <Card.Img variant="top" src="http://askavy.com/demo/img/img-card.jpg" />
        <Card.Body>
          <Card.Title>Card title </Card.Title>
          <Card.Text>
            Card Text This card has supporting text below as a natural lead-in
            to additional content.{" "}
          </Card.Text>
        </Card.Body>
        <Card.Footer>
          <small className="text-muted">Last updated 10 mins ago</small>
        </Card.Footer>
      </Card>

      <Card>
        <Card.Img variant="top" src="http://askavy.com/demo/img/img-card.jpg" />
        <Card.Body>
          <Card.Title>Card title</Card.Title>
          <Card.Text>
            Card Text his card has supporting text below as a natural lead-in to
            additional content.{" "}
          </Card.Text>
        </Card.Body>
        <Card.Footer>
          <small className="text-muted">Last updated 10 mins ago</small>
        </Card.Footer>
      </Card>

      <Card>
        <Card.Img variant="top" src="http://askavy.com/demo/img/img-card.jpg" />
        <Card.Body>
          <Card.Title>Card title</Card.Title>
          <Card.Text>
            Card Text his card has supporting text below as a natural lead-in to
            additional content.{" "}
          </Card.Text>
        </Card.Body>
        <Card.Footer>
          <small className="text-muted">Last updated 11 mins ago</small>
        </Card.Footer>
      </Card>
    </CardColumns>
  );
}
function App() {
  return (
    <div>
      <CardDisplay />
    </div>
  );
}

export default App;

```

<h2>React Card – Bootstrap 4 and Material Design</h2>


```javascript

import React from "react";
import "bootstrap/dist/css/bootstrap.min.css";
import "mdbreact/dist/css/mdb.css";
import "@fortawesome/fontawesome-free/css/all.min.css";
import {
  MDBBtn,
  MDBCard,
  MDBCardBody,
  MDBCardImage,
  MDBCardTitle,
  MDBCardText,
  MDBRow,
  MDBCol,
  MDBIcon,
} from "mdbreact";

const CardMaterail = () => {
  return (
    <MDBRow>
      <MDBCol md="4">
        <MDBCard cascade>
          <MDBCardImage
            cascade
            className="img-fluid"
            overlay="white-light"
            hover
            src="http://askavy.com/demo/img/img-card.jpg"
          />
          <MDBBtn
            floating
            tag="a"
            className="ml-auto mr-4 lighten-3 mdb-coalor"
            action
          >
            <MDBIcon icon="chevron-right" />
          </MDBBtn>
          <MDBCardBody cascade>
            <MDBCardTitle>Card title</MDBCardTitle>
            <hr />
            <MDBCardText>
              Some quick example text to build on the card title and make up the
              bulk of the card's content.
            </MDBCardText>
          </MDBCardBody>
          <div className="rounded-bottom mdb-color lighten-3 text-center pt-3">
            <ul className="list-unstyled list-inline font-small">
              <li className="list-inline-item pr-2 white-text">
                <MDBIcon far icon="clock" /> 05/10/2015
              </li>
              <li className="list-inline-item pr-2">
                <a href="#!" className="white-text">
                  <MDBIcon far icon="comments" className="mr-1" />
                  12
                </a>
              </li>
              <li className="list-inline-item pr-2">
                <a href="#!" className="white-text">
                  <MDBIcon fab icon="facebook-f" className="mr-1" />
                  21
                </a>
              </li>
              <li className="list-inline-item">
                <a href="#!" className="white-text">
                  <MDBIcon fab icon="twitter" className="mr-1" />5
                </a>
              </li>
            </ul>
          </div>
        </MDBCard>
      </MDBCol>
    </MDBRow>
  );
};

export default CardMaterail;

```



