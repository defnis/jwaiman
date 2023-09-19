# Hello!! My name is Jose Waiman.  👋

### Full Stack Developer student with React JS and Artifitial Intelligence

In 2014, I started my professional career is Tourism.

I worked for more than 10 years in Patagonia Argentina. After the pandemic of the year 2020, I returned to my hometown and started the beautiful path of Programming. During my studies I have started web layout (HTML5, CSS3, Javascript, React and Node), C# oriented to Videogames, various programming logic courses, and currently studying Python, R and MySQL, oriented to Databases.

I consider myself a responsible, proactive person, with many gains from learning and sharing knowledge.

## Technologies:
[![HTML5](https://img.shields.io/badge/HTML5-ef8952?style=for-the-badge&logo=HTML5&logoColor=white&labelColor=101010)]()
[![CSS3](https://img.shields.io/badge/CSS3-63ecbe?style=for-the-badge&logo=CSS3&logoColor=white&labelColor=101010)]()
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=white&labelColor=101010)]()
[![React](https://img.shields.io/badge/React-F788eE?style=for-the-badge&logo=react&logoColor=white&labelColor=101010)]()
[![Python](https://img.shields.io/badge/Python-63e5ec?style=for-the-badge&logo=python&logoColor=white&labelColor=101010)]()
[![R](https://img.shields.io/badge/R-4479A1?style=for-the-badge&logo=R&logoColor=white&labelColor=101010)]()
[![MySQL](https://img.shields.io/badge/MySQL-ec6381?style=for-the-badge&logo=mysql&logoColor=white&labelColor=101010)]()</br>
[![Java](https://img.shields.io/badge/Java-17DF9E?style=for-the-badge&logo=java&logoColor=yellow&labelColor=101010)]()

## Code Sample

#### React Code

```react
import React from "react";
import { BrowserRouter, Routes, Route } from "react-router-dom";

import Header from './components/layout/Header';
import Nav from './components/layout/Nav';
import Footer from './components/layout/Footer';

import Contacto from './pages/Contacto';
import Home from './pages/Home';
import Novedades from './pages/Novedades';
import Nosotros from './pages/Nosotros';
import LoginForm from "./pages/Loginform";

function App() {
  return (
    <div className="App">
        <Header />

        <BrowserRouter>
            <Nav />
            <Routes>
              <Route path="/" element={<Home />}/>
              <Route path="/nosotros" element={<Nosotros />}/>
              <Route path="/novedades" element={<Novedades />}/>
              <Route path="/contacto" element={<Contacto />}/>
              <Route path="/loginform" element={<LoginForm />}/>
            </Routes>
        </BrowserRouter>
        <Footer />
    </div>
  );
}

export default App;
```

#### Node Code
```node
var createError = require('http-errors');
var express = require('express');
var path = require('path');
var cookieParser = require('cookie-parser');
var logger = require('morgan');
var fileupload = require('express-fileupload');

require('dotenv').config();
var session = require('express-session');

var indexRouter = require('./routes/index');
var usersRouter = require('./routes/users');
var loginRouter = require('./routes/admin/login');
var adminRouter = require('./routes/admin/novedades');

var app = express();

var nosotrosRouter = require('./routes/nosotros');
app.use('./nosotros', nosotrosRouter);

// view engine setup
app.set('views', path.join(__dirname, 'views'));
app.set('view engine', 'hbs');

app.use(logger('dev'));
app.use(express.json());
app.use(express.urlencoded({ extended: false }));
app.use(cookieParser());
app.use(express.static(path.join(__dirname, 'public')));

app.use(session({
  secret: 'Pw2021awqyeudj',
  cookie: {maxAge:null},
  reserve: false,
  saveUninitialized: true
}))

secured = async(req, res, next) => {
  try {
    console.log(req.session.id.usuario);
    if (req.session.id.usuario) {
      next();
    } else {
      res.redirect('/admin/login');
    } //Cierro else
  } catch (error) {
    console.log(error);
  } //Cierro Catch
} //Cierro Secured

app.use(fileupload ({
  useTempFiles: true,
  tempFileDir: '/tmp/'
}));
```

#### Python Code

```python
import pandas as pd

rfc=pd.Series({'Usuario1':'COG786588', 'Usuario2': 'GUHA457684'})

rfc.str.match(r'\w{4}\d{6}')

rfc

```
```python
class A():
    def __init__(self):
        self.cuenta = 0 
        self.contador = 0
    
    @property  #Le decimos a python que llamo a un metodo GET. 
    def cuenta(self):
        return self._cuenta
    
    @property
    def contador(self):
        return self._contador


a = A()
print(a.cuenta)
print(a.contador)
```


## Meet me at:

[YouTube](https://www.youtube.com/channel/UCg2u_oeoLUSNVrbf46KWy6Q), [Twitch](https://www.twitch.tv/soy_defnis), [Twitter](https://twitter.com/jwaiman243), [Instagram](https://instagram.com/josewaiman), [TikTok](https://tiktok.com/@soy_defnis), [Facebook](https://www.facebook.com/jose.waiman), [LinkedIn](https://www.linkedin.com/in/josé-waiman-bba61757/)



