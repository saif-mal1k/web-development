
### image




### code
```html
<html>

<head>
  <link rel="stylesheet" type="text/css" href="./style.css">
  <style>
    .theme-light {
      --bg: #f5f6f7;
      --bg-alt: #fff;
      --fg: #444;
      --fg-alt: #222;
      --primary: #306cc4;
      --primary-alt: #185dc7;
      --primary-light: rgba(44, 93, 206, 0.1);
      --container-shadow: 0 2px 4px rgb(0 0 0 / 10%);
    }


    .theme-dark {
      --bg: #0f0840;
      --bg-alt: rgb(22 28 41 / 33%);
      --fg: #bdbddd;
      --fg-alt: #cdcdff;
      --primary: #807ae8;
      --primary-alt: #706aec;
      --primary-light: rgb(18 17 49 / 44%);
      --container-shadow: rgba(0, 0, 0, 0.1) 0px 4px 6px -1px,
        rgba(0, 0, 0, 0.06) 0px 2px 4px -1px;
    }


    body {
      background-color: var(--color-secondary);
      color: var(--font-color);
    }


    /* The switch - the box around the slider */
    .switch {
      position: relative;
      display: inline-block;
      width: 60px;
      height: 20px;
    }

    /* Hide default HTML checkbox */
    .switch input {
      opacity: 0;
      width: 0;
      height: 0;
    }

    /* The slider */
    .slider {
      position: absolute;
      cursor: pointer;
      top: 0;
      left: 0;
      right: 0;
      bottom: 0;
      background-color: white;
      -webkit-transition: 0.4s;
      transition: 0.4s;
    }


    input:checked+.slider {
      background-color: black;
    }

    input:focus+.slider {
      box-shadow: 0 0 1px black;
    }



    /* Rounded sliders */
    .slider.round {
      border-radius: 34px;
    }

    .slider.round:before {
      border-radius: 50%;
    }
  </style>
  <link rel="icon" href="https://linktomyimage.jpg" type="image/icon type">
  <title>
    My Name
  </title>
  <style>
    /* table of contents */

    /* 1. variables*/
    /* 2. global styles */
    /* 3. layout */
    /* 4. components */
    /* 5. utilities */

    /* ================
	 1. variables
   ================ */


    /* =====================
     2. global styles
   ===================== */

    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
      border: 0;
      box-shadow: none;
    }

    ::-moz-selection {
      background: var(--primary);
      color: var(--bg);
    }

    ::-webkit-selection,
    ::selection {
      background: var(--primary);
      color: var(--bg);
    }

    ::-webkit-scrollbar {
      width: 16px;
    }

    ::-webkit-scrollbar-track {
      background-color: var(--bg-alt);
    }

    ::-webkit-scrollbar-thumb {
      border: 4px solid var(--bg);
      background-color: var(--primary);
      border-radius: 0.5em;
    }

    ::-webkit-scrollbar-thumb:hover {
      background-color: var(--primary-alt);
    }

    html {
      scroll-behavior: smooth;
    }

    body {
      margin: 0 auto;
      max-width: 1100px;
      width: 95%;
      background-color: var(--bg);
      color: var(--fg);
      font-family: 'Poppins', sans-serif;
      line-height: 1.5;
      transition: background-color 0.1s linear;
    }

    h1,
    h2,
    h3,
    h4 {
      color: var(--fg-alt);
      line-height: 1.1;
    }

    h1 {
      font-size: 5rem;
    }

    h2 {
      font-size: 1.8em;
    }

    ul {
      list-style-type: none;
    }

    button {
      cursor: pointer;
      font-family: inherit;
      background-color: inherit;
    }

    a {
      text-decoration: none;
    }

    .link {
      padding: 0 0 0.12em 0;
      position: relative;
      color: var(--primary);
    }

    .link:hover {
      color: var(--primary);
    }

    .link:active {
      color: var(--primary-alt);
    }

    .link::before {
      content: '';
      display: inline;
      width: 0%;
      height: 0.12em;
      position: absolute;
      bottom: 0;
      background-color: var(--primary);
      transition: width 0.2s ease-out;
    }

    .link:hover::before {
      width: 100%;
    }

    @media (max-width: 768px) {
      h1 {
        font-size: 4rem;
      }
    }

    @media (max-width: 580px) {
      h2 {
        font-size: 1.5rem;
      }
    }

    @media (max-width: 320px) {
      h1 {
        font-size: 3rem;
      }
    }

    /* =============
     3. layout
   ============= */

    header,
    nav,
    nav ul,
    .hero,
    .contact ul,
    footer {
      display: flex;
      align-items: center;
    }

    header {
      height: 6em;
      justify-content: space-between;
    }

    nav li {
      font-weight: 500;
      margin: 0 0.5em;
    }

    .hero {
      margin-top: 6em;
      justify-content: space-between;
    }

    .hero h1 {
      display: flex;
      flex-direction: column;
      flex-basis: 50%;
    }

    .hero-name {
      color: var(--primary);
    }

    .hero-about {
      flex-basis: 40%;
    }

    .hero-about p {
      font-size: 1.1rem;
    }

    .hero-about .btn {
      margin-top: 2.2em;
    }

    section {
      margin-top: 5em;
    }

    .section-title {
      padding-top: 0.5em;
      margin-bottom: 1.5em;
      text-align: center;
      text-transform: uppercase;
    }

    .section-title::after {
      content: '';
      margin: 0.3em auto 0 auto;
      display: block;
      width: 1.5em;
      border-bottom: 0.2em solid var(--primary);
    }

    .project-container {
      display: flex;
      justify-content: space-between;
      align-items: center;
      background-color: var(--bg-alt);
      max-width: 950px;
      width: 95%;
      margin: 2em auto;
      padding: 2em;
      text-align: center;
      box-shadow: var(--container-shadow);
      border-radius: 1em;
    }

    .project img {
      border-radius: 0.5em;
    }

    .project-content {
      flex-basis: 50%;
      margin-left: 2em;
    }

    .project-content p {
      margin: 1.2em 0;
    }

    .project-skill,
    .project-link {
      display: flex;
      justify-content: center;
      flex-wrap: wrap;
    }

    .project-skill {
      margin: 0 auto;
    }

    .project-skill li {
      font-size: 0.8rem;
      font-weight: 700;
      margin: 0.3em 0.2em;
      padding: 0.4em 0.6em;
      border-radius: 5em;
      background-color: var(--primary-light);
      color: var(--primary-alt);
    }

    .project-link {
      margin-top: 1.2em;
    }

    .stack-container {
      margin: 0 auto;
      display: flex;
      gap: 1em;
      flex-wrap: wrap;
      justify-content: center;
      align-items: center;
    }

    .tech-container {
      width: 10em;
      height: 10em;
      position: relative;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      background-color: var(--bg-alt);
      border-radius: 1.5em;
      box-shadow: var(--container-shadow);
      overflow: hidden;
      font-size: 0.8rem;
      font-weight: 500;
    }

    .tech-container::before {
      content: '';
      position: absolute;
      bottom: 0px;
      left: 0px;
      transform: scaleX(0);
      width: 100%;
      height: 6px;
      border-radius: 1.5;
      background-color: var(--primary-alt);
      transition: all 0.2s linear;
    }

    .tech-container:hover::before {
      transform: scaleX(1);
    }

    .tech-container i {
      font-size: 3rem;
      margin-bottom: 0.2em;
    }

    .contact ul {
      flex-wrap: wrap;
      justify-content: center;
    }

    .contact .btn {
      margin-right: 0.5em;
      margin-top: 0.3em;
    }

    .contact .icon,
    .hero .icon {
      margin-right: 0.2em;
    }

    footer {
      margin-top: 5em;
      height: 7em;
      flex-direction: column;
      justify-content: center;
      position: absolute;
      left: 0;
      right: 0;
      background-color: var(--bg-alt);
      box-shadow: 0 -0.1em 1em rgb(0, 0, 0, 0.1);
    }

    footer ul {
      display: flex;
    }

    footer small {
      font-weight: 500;
      margin-top: 0.5em;
    }

    @media (max-width: 950px) {
      .project-container {
        flex-direction: column;
        max-width: 450px;
        padding: 1.5em;
      }

      .project img {
        max-width: 100%;
        max-height: 100%;
        margin: 0 auto;
        margin-bottom: 2em;
      }

      .project-content {
        padding: 0;
        margin-left: 0;
      }
    }

    @media (max-width: 580px) {
      nav ul {
        flex-direction: column;
        padding: 4em 0;
        position: absolute;
        right: 0;
        left: 0;
        top: 5em;
        background-color: var(--bg);
        width: 0;
        overflow: hidden;
        transition: width 0.2s ease-in-out;
      }

      .display-nav-list {
        width: 100%;
      }

      nav li {
        margin: 0.5em 0;
      }

      .hero,
      .hero-about,
      section {
        margin-top: 2.5em;
      }

      .hero {
        padding-bottom: 1em;
        flex-direction: column;
      }

      .hero h1,
      .hero-about {
        width: 100%;
      }

      .project .section-title {
        margin-bottom: 0;
      }

      .stack-container i {
        font-size: 3rem;
      }
    }

    /* =================
     4. components
   ================= */

    /* buttons */

    .btn {
      display: inline-block;
      border-radius: 5em;
      font-size: 0.8rem;
      font-weight: 600;
      transition: transform 0.2s ease-in-out;
      padding: 1em 1.6em;
      background-color: var(--primary);
      color: var(--bg);
    }

    .btn:hover {
      background-color: var(--primary-alt);
    }

    .btn:active {
      transform: translateY(-0.4em);
    }

    /* icons */

    .icon-normal,
    .icon-border {
      margin: 0.2em;
      display: flex;
      align-items: center;
      justify-content: center;
      position: relative;
      z-index: 1;
      cursor: pointer;
      border-radius: 50%;
      font-size: 1.2rem;
    }

    .icon-normal:hover,
    .icon-border:hover {
      color: var(--bg);
    }

    .icon-normal::after,
    .icon-border::after {
      content: '';
      position: absolute;
      width: 0%;
      height: 0%;
      z-index: -1;
      background-color: var(--primary);
      border-radius: 50%;
      transition: all 0.25s ease-in-out;
    }

    .icon-normal:hover::after,
    .icon-border:hover::after {
      width: 100%;
      height: 100%;
      border: 0.2em solid var(--primary);
    }

    .icon-normal {
      width: 1.6em;
      height: 1.6em;
      color: var(--fg-alt);
    }

    .icon-border {
      width: 2.2em;
      height: 2.2em;
      color: var(--primary);
      border: 0.15em solid var(--primary);
    }

    /* icons */

    .scroll-container {
      display: flex;
      justify-content: flex-end;
    }

    .scroll-up {
      display: none;
      position: fixed;
      font-size: 0.9rem;
      bottom: 3em;
      right: 2em;
      font-weight: 600;
      transition: transform 0.2s ease-in-out;
    }

    .scroll-up:active {
      transform: translateY(0.4em);
    }

    .scroll-up a {
      background-color: var(--primary);
      padding: 0.9em 1.2em;
      color: var(--bg);
      border-radius: 50%;
    }

    .scroll-up a:hover {
      background-color: var(--primary-alt);
    }

    @media (max-width: 1000px) {
      .scroll-container {
        display: none;
      }
    }

    /* ============
   5. utilities
   ============ */

    .fa-bars {
      display: none;
    }

    .header-title {
      font-weight: 700;
      text-shadow: 0 4px 2px rgba(0, 0, 0, 0.2);
    }

    nav .link {
      color: var(--fg-alt);
    }

    @media (max-width: 580px) {
      .fa-bars {
        display: flex;
      }
    }

    Footer

    /* Teams section styling */
    .teams .title::after {
      content: "Who with me";
    }

    .teams .carousel .card {
      background: #222;
      border-radius: 6px;
      padding: 25px 35px;
      text-align: center;
      transition: all 0.3s ease;
    }

    .card{
      height: 360px !important;
        }

    .teams .carousel .card:hover {
      background: var(--primary);
    }

    .teams .carousel .card:hover .box {
      transform: scale(1.05);
    }

    .teams .carousel .card .box {
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;

    }

    .teams .carousel .card .text {
      font-size: 25px;
    }

    .teams .carousel .card img {
      height: 150px;
      width: 150px;
      object-fit: cover;
      border-radius: 50%;
      border: 5px solid var(--primary);

    }

    .teams .carousel .card:hover img {
      border-color: #fff;
    }

    .owl-dots {
      text-align: center;
      margin-top: 20px;

    }

    .owl-dot {
      height: 13px;
      width: 13px;
      margin: 0 5px;
      outline: none ! important;
      border-radius: 50%;
      border: 2px solid var(--primary) !important;
      transition: all 0.3s ease;
    }

    .owl-dot.active {
      width: 35px;
      border-radius: 14px;
    }

    .owl-dot.active,
    .owl-dot:hover {
      background: var(--primary) !important;
    }

    /* contact section styling */
    .contact .title::after {
      content: "Get in touch";
    }

    .contact .content-content .column {
      width: calc(50% - 30px);
    }

    .contact .content-content .text {
      font-size: 20px;
      font-weight: 600;
      margin-bottom: 10px;
    }

    .contact .content-content .left p {
      text-align: justify;
    }

    .contact .content-content .left .icons {
      margin: 10px 0;
    }

    .contact .content-content .row {
      display: flex;
      height: 65px;
      align-items: center;
    }

    .contact .content-content .row .info {
      margin-left: 30px;


    }

    .contact .content-content .row i {
      font-size: 25px;
      color: var(--primary);
    }

    .contact .content-content .info .head {
      font-weight: 500;
    }


    .contact .content-content .info .sub-title {
      color: #b0acac82;
    }


    .contact .right form .fields {
      display: flex;
    }


    .contact .right form .fields .field,
    .contact .right form .field {
      height: 45px;
      width: 100%;
      margin-bottom: 15px;
    }

    .contact .right form .field .textarea {
      height: 80px;
      width: 100%;
    }

    .contact .right form .field .name {
      margin-right: 10px;
    }

    .contact .right form .field .email {
      margin-left: 10px;
    }

    .contact .right form .field input,
    .contact .right form .textarea textarea {
      height: 100%;
      width: 100%;
      border: 1px solid lightgrey;
      border-radius: 6px;
      border-radius: 6px;
      outline: none;
      padding: 0 15px;
      font-size: 17px;
      font-family: 'Poppins', sans-serif;

    }

    .contact .right form .textarea textarea {
      padding-top: 10px;
      resize: none;

    }

    .contact .right form .button {
      height: 47px;
      width: 170px;
    }

    .contact .right form .button button {
      width: 100%;
      height: 100%;
      background: var(--primary);
      border: 2px solid var(--primary);
      color: #fff;
      font-size: 20px;
      border-radius: 6px;
      font-weight: 500;
      font-family: 'Ubuntu', sans-serif;
      cursor: pointer;
      transition: all 0.3s ease;
    }

    .contact .right form .button button:hover {
      color: var(--primary);
      background: none;
    }
  </style>

  <style>
    @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@400;500;600;700&family=Ubuntu:ital,wght@0,400;0,700;1,500&display=swap');


    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      text-decoration: none;

    }

    html {
      scroll-behavior: smooth;
    }

    .max-width {
      max-width: 1300px;
      /*padding: 0 80px;*/
      margin: auto;
    }

    .scroll-up-btn {
      position: fixed;
      height: 45px;
      width: 42px;
      background: var(--primary);
      right: 30px;
      bottom: 30px;
      text-align: center;
      line-height: 45px;
      color: #fff;
      z-index: 999;
      font-size: 30px;
      border-radius: 6px;
      cursor: pointer;
      opacity: 0;
      pointer-events: none;
      transition: all 0.3s ease;
    }

    .scroll-up-btn .show {
      bottom: 30px;

      opacity: 1;
      pointer-events: auto;


    }

    /* navbar styling */
    .navbar {

      position: fixed;
      z-index: 999;
      /* background-color: crimson; */
      padding: 30px 0;
      width: 100%;
      font-family: 'Ubuntu', 'sans-serif';
      transition: all 0.3s ease;

    }

    .navbar.sticky {
      /* position: fixed; */
      background-color: var(--primary);
      padding: 30px 0;
      /* width: 100%; */
      font-family: 'Ubuntu', 'sans-serif';


    }

    .navbar .max-width {
      display: flex;
      align-items: center;
      justify-content: space-between;

    }

    .navbar .logo a {
      color: #fff;
      font-size: 35px;
      font-weight: 600;

    }

    .navbar .logo a span {


      color: var(--primary);

    }

    .navbar.sticky .logo a span {
      color: #fff;
      transition: all 0.3s ease;

    }

    .navbar .menu li {
      list-style: none;
      display: inline-block;
    }

    .navbar .menu li a {
      color: #fff;
      font-size: 18px;
      font-weight: 500;
      margin-left: 25px;
      /* text-decoration: none; */
      transition: color 0.3s ease;
    }

    .navbar .menu li a:hover {
      color: var(--primary);
    }

    .navbar.sticky .menu li a:hover {
      color: black;
      transition: all 0.3s ease;

    }

    /* Menu button styling */
    .menu-btn {
      color: #fff;
      font-size: 23px;
      cursor: pointer;
      display: none;
    }


    /* home section styling */
    .home {
      display: flex;

      background-image: url("https://i.ibb.co/HqyWx5M/image-2022-07-26-202353220.png");

      background-repeat: no-repeat;
      background-position: center;
      height: 100vh;
      background-size: cover;
      background-attachment: fixed;
      color: #fff;
      min-height: 500px;
      font-family: 'Ubuntu', 'sans-serif';

    }

    .home .max-width {
      margin: auto 0 auto 40px;
    }

    .home .home-content .text-1 {
      font-size: 27px;
    }

    .home .home-content .text-2 {
      font-size: 75px;
      font-weight: 600;
      margin-left: -3px;
    }

    .home .home-content .text-3 {
      font-size: 40px;
      margin: 5px 0;
    }

    .home .home-content .text-3 span {
      color: var(--primary);
      font-weight: 500;
    }

    .home .home-content a {
      display: inline-block;
      background: var(--primary);
      color: #fff;
      font-size: 25px;
      padding: 12px 36px;
      margin-top: 20px;
      border-radius: 6px;
      border: 2px solid var(--primary);
      transition: all 0.3s ease-out;
    }

    .home .home-content a:hover {
      color: #fff;
      background: none;
    }

    /* all similar contant styling code */
    .about,
    .services,
    .skills,
    .teams,
    .contact,
    footer {
      font-family: 'Poppins', sans-serif;

    }

/*    section {
      padding: 100px 0;


    }*/

    .about .about-content,
    .services .serv-content,
    .skills .skills-content,
    .content-content {
      display: flex;
      flex-wrap: wrap;
      align-items: center;
      justify-content: space-between;
    }

    section .title {
      position: relative;
      text-align: center;
      font-size: 40px;
      font-weight: 500;
      margin-bottom: 60px;
      padding-bottom: 20px;
      font-family: 'Ubuntu', sans-serif;
    }

    section .title::before {
      content: "";
      position: absolute;
      bottom: 0px;
      left: 50%;
      width: 180px;
      height: 3px;
      background: #111;
      transform: translateX(-50%);
    }

    section .title::after {

      position: absolute;
      bottom: -12px;
      left: 50%;
      padding: 5px;
      font-size: 20px;
      color: var(--primary);

      padding: 5px;
      background: #fff;
      transform: translateX(-50%);
    }

    /*  about section styling */





    .about .title::after {
      content: "who i am";
    }


    .about .about-content .left {
      width: 45%;

    }

    .about .about-content .left img {
      height: 400px;
      width: 400px;
      object-fit: cover;
      border-radius: 6px;
    }

    .about .about-content .right {
      width: 55%;

    }

    .about .about-content .right .text {
      font-size: 25px;
      font-weight: 600;
      margin-bottom: 10px;

    }

    .about .about-content .right .text span {
      color: var(--primary);

    }

    .about .about-content .right p {
      text-align: justify;

    }

    .about .about-content .right a {
      display: inline-block;
      background: var(--primary);
      color: #fff;
      font-size: 20px;
      font-weight: 500;
      padding: 10px 30px;
      margin-top: 20px;
      border-radius: 6px;
      border: 2px solid var(--primary);
      transition: all 0.3s ease-out;

    }

    .about .about-content .right a:hover {
      color: var(--primary);
      background: none;
    }


    /* services section stylings */



    .services,
    .teams {
      color: #fff;
      background:rgb(17 17 17 / 0%);

    }

    .services .title::before,
    .teams .title::before {
      background: #fff;
    }

    .services .title::after,
    .teams .title::after {
      background: #111;
      content: "what i provide";
    }

    .services .serv-content .card {
      width: calc(33% - 20px);
      background: #222;
      text-align: center;
      border-radius: 6px;
      padding: 20px 25px;
      cursor: pointer;
    }

    .services .serv-content .card:hover {
      background: var(--primary);
    }

    .services .serv-content .card .box {
      transition: all 0.3s ease;
    }

    .services .serv-content .card:hover .box {
      transform: scale(1.05);
    }

    .services .serv-content .card i {
      font-size: 50px;
      color: var(--primary);
      transition: color 0.3s ease;
    }

    .services .serv-content .card:hover i {
      color: #fff;

    }

    .services .serv-content .card .text {
      font-size: 25px;
      font-weight: 500;
      margin: 10px 0 7px 0;
    }

    /* skills section styling */

    .skills .title::after {
      content: "what i know";
    }

    .skills .skills-content .column {
      width: calc(50% - 30px);
    }

    .skills .skills-content .left .text {
      font-size: 25px;
      font-weight: 600;
      margin-bottom: 10px;
    }

    .skills .skills-content .left p {
      text-align: justify;

    }

    .skills .skills-content .left a {
      display: inline-block;
      background: var(--primary);
      color: #fff;
      font-size: 18px;
      font-weight: 500;
      padding: 8px 16px;
      margin-top: 20px;
      border-radius: 6px;
      border: 2px solid var(--primary);
      transition: all 0.3s ease-out;

    }

    .skills .skills-content .left a:hover {
      color: var(--primary);
      background: none;
    }

    .skills .skills-content .right .bars {
      margin-bottom: 15px;
    }

    .skills .skills-content .right .info {
      display: flex;
      margin-bottom: 5px;
      align-items: center;
      justify-content: space-between;
    }


    .skills .skills-content .right span {
      font-weight: 500;
      font-size: 18px;
    }

    .skills .skills-content .right .line {
      width: 5px;
      width: 100%;
      background: lightgrey;
      position: relative;

    }

    .skills .skills-content .right .line::before {
      content: "";
      position: absolute;
      height: 100%;

      left: 0;
      top: 0;
      background: var(--primary);
      transition: all 0.3s ease-in-out;
    }


    .skills .skills-content .right .html::before {
      width: 90%;
    }

    .skills .skills-content .right .css::before {
      width: 90%;
    }

    .skills .skills-content .right .js::before {
      width: 50%;
    }

    .skills .skills-content .right .php::before {
      width: 40%;
    }

    .skills .skills-content .right .mysql::before {
      width: 70%;
    }

    /* Teams section styling */
    .teams .title::after {
      content: "Who with me";
    }

    .teams .carousel .card {
      background: #222;
      border-radius: 6px;
      padding: 25px 35px;
      text-align: center;
      transition: all 0.3s ease;
    }

    .teams .carousel .card:hover {
      background: var(--primary);
    }

    .teams .carousel .card:hover .box {
      transform: scale(1.05);
    }

    .teams .carousel .card .box {
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;

    }

    .teams .carousel .card .text {
      font-size: 25px;
    }

    .teams .carousel .card img {
      height: 150px;
      width: 150px;
      object-fit: cover;
      border-radius: 50%;
      border: 5px solid;

    }

    .teams .carousel .card:hover img {
      border-color: #fff;
    }

    .owl-dots {
      text-align: center;
      margin-top: 20px;

    }

    .owl-dot {
      height: 13px;
      width: 13px;
      margin: 0 5px;
      outline: none ! important;
      border-radius: 50%;
      border: 2px solid !important;
      transition: all 0.3s ease;
    }

    .owl-dot.active {
      width: 35px;
      border-radius: 14px;
    }

    .owl-dot.active,
    .owl-dot:hover {
      background: var(--primary) !important;
    }

    /* contact section styling */
    .contact .title::after {
      content: "Get in touch";
    }

    .contact .content-content .column {
      width: calc(50% - 30px);
    }

    .contact .content-content .text {
      font-size: 20px;
      font-weight: 600;
      margin-bottom: 10px;
    }

    .contact .content-content .left p {
      text-align: justify;
    }

    .contact .content-content .left .icons {
      margin: 10px 0;
    }

    .contact .content-content .row {
      display: flex;
      height: 65px;
      align-items: center;
    }

    .contact .content-content .row .info {
      margin-left: 30px;


    }

    .contact .content-content .row i {
      font-size: 25px;
      color: var(--primary);
    }

    .contact .content-content .info .head {
      font-weight: 500;
    }


    .contact .content-content .info .sub-title {
      color: #8e8e8eb9;
    }


    .contact .right form .fields {
      display: flex;
    }


    .contact .right form .fields .field,
    .contact .right form .field {
      height: 45px;
      width: 100%;
      margin-bottom: 15px;
    }

    .contact .right form .field .textarea {
      height: 80px;
      width: 100%;
    }

    .contact .right form .field .name {
      margin-right: 10px;
    }

    .contact .right form .field .email {
      margin-left: 10px;
    }

    .contact .right form .field input,
    .contact .right form .textarea textarea {
      height: 100%;
      width: 100%;
      border: 1px solid lightgrey;
      border-radius: 6px;
      border-radius: 6px;
      outline: none;
      padding: 0 15px;
      font-size: 17px;
      font-family: 'Poppins', sans-serif;

    }

    .contact .right form .textarea textarea {
      padding-top: 10px;
      resize: none;

    }

    .contact .right form .button {
      height: 47px;
      width: 170px;
    }

    .contact .right form .button button {
      width: 100%;
      height: 100%;
      background: var(--primary);
      border: 2px solid var(--primary);
      color: #fff;
      font-size: 20px;
      border-radius: 6px;
      font-weight: 500;
      font-family: 'Ubuntu', sans-serif;
      cursor: pointer;
      transition: all 0.3s ease;
    }

    .contact .right form .button button:hover {
      color: var(--primary);
      background: none;
    }

    /* footer section styling */
    footer {
      background: #111;
      padding: 20px 23px;
      color: #fff;
      text-align: center;
    }

    footer span a {
      color: var(--primary);
    }

    footer span a:hover {
      text-decoration: none;
    }






    /* responsive media query start*/
    @media(max-width:1300px) {

      .home .max-width {
        margin-left: 0px;
      }

    }

    @media(max-width:1104px) {
      .about .about-content .left img {
        height: 350px;
        width: 350px;
      }

    }

    @media(max-width:991px) {
      .max-width {

        padding: 0 50px;

      }
    }


    @media(max-width:947px) {



      .menu-btn {
        display: block;
        z-index: 999;

      }

      .menu-btn i.active::before {
        content: "\f00d";
      }

      .navbar .menu {
        position: fixed;
        height: 100vh;
        width: 100%;
        left: -100%;
        top: 0;
        background: #111;
        text-align: center;
        padding-top: 80px;
        transition: all 0.3s ease-in-out;

      }

      .navbar .menu.active {
        left: 0;
      }

      .navbar .menu li {
        display: block;
      }

      .navbar .menu li a {
        display: inline-block;
        margin: 20px 0;
        font-size: 25px;
      }


      .home .home-content .text-2 {
        font-size: 70px;

      }

      .home .home-content .text-3 {
        font-size: 35px;

      }

      .home .home-content a {
        font-size: 23px;
        padding: 10px 30px;
      }

      .max-width {
        max-width: 800px;

      }

      .about .about-content .column {
        width: 100%;
      }

      .about .about-content .left {
        display: flex;
        justify-content: center;
        margin: 0 auto 60px;

      }

      .about .about-content .right {
        flex: 100%;

      }

      .services .serv-content .card {
        width: calc(50% - 10px);
        margin-bottom: 20px;
      }

      .skills .skills-content .column,
      .contact .content-content .column {
        width: 100%;
        margin-bottom: 35px;
      }



    }

    @media(max-width:690px) {

      .max-width {

        padding: 0 23px;

      }

      .home .home-content .text-2 {
        font-size: 60px;

      }

      .home .home-content .text-3 {
        font-size: 32px;

      }

      .home .home-content a {
        font-size: 20px;
        /* padding: 9px 25px; */
      }

      .services .serv-content .card,
      .skills .skills-content .column {
        width: 100%;
      }
    }

    @media(max-width:500px) {

      .max-width {

        padding: 0 23px;

      }

      .home .home-content .text-2 {
        font-size: 50px;

      }

      .home .home-content .text-3 {
        font-size: 27px;

      }

    }
  </style>

  <style>
    .csslider {
      -moz-perspective: 1300px;
      -ms-perspective: 1300px;
      -webkit-perspective: 1300px;
      perspective: 1300px;
      display: inline-block;
      text-align: left;
      position: relative;
      margin-bottom: 22px;
    }

    .csslider>input {
      display: none;
    }

    .csslider>input:nth-of-type(10):checked~ul li:first-of-type {
      margin-left: -900%;
    }

    .csslider>input:nth-of-type(9):checked~ul li:first-of-type {
      margin-left: -800%;
    }

    .csslider>input:nth-of-type(8):checked~ul li:first-of-type {
      margin-left: -700%;
    }

    .csslider>input:nth-of-type(7):checked~ul li:first-of-type {
      margin-left: -600%;
    }

    .csslider>input:nth-of-type(6):checked~ul li:first-of-type {
      margin-left: -500%;
    }

    .csslider>input:nth-of-type(5):checked~ul li:first-of-type {
      margin-left: -400%;
    }

    .csslider>input:nth-of-type(4):checked~ul li:first-of-type {
      margin-left: -300%;
    }

    .csslider>input:nth-of-type(3):checked~ul li:first-of-type {
      margin-left: -200%;
    }

    .csslider>input:nth-of-type(2):checked~ul li:first-of-type {
      margin-left: -100%;
    }

    .csslider>input:nth-of-type(1):checked~ul li:first-of-type {
      margin-left: 0%;
    }

    .csslider>ul {
      position: relative;
      width: 820px;
      height: 380px;
      z-index: 1;
      font-size: 0;
      line-height: 0;
      background-color: #d1d1d1;
      border: 10px solid #d1d1d1;
      margin: 0 auto;
      padding: 0;
      overflow: hidden;
      white-space: nowrap;
      -moz-box-sizing: border-box;
      -webkit-box-sizing: border-box;
      box-sizing: border-box;
    }

    .csslider>ul>li {
      position: relative;
      display: inline-block;
      width: 800px;
      min-height: 360px;
      overflow: hidden;
      font-size: 15px;
      font-size: initial;
      line-height: normal;
      -moz-transition: all 0.5s cubic-bezier(0.4, 1.3, 0.65, 1);
      -o-transition: all 0.5s ease-out;
      -webkit-transition: all 0.5s cubic-bezier(0.4, 1.3, 0.65, 1);
      transition: all 0.5s cubic-bezier(0.4, 1.3, 0.65, 1);
      -moz-background-size: cover;
      -o-background-size: cover;
      -webkit-background-size: cover;
      background-size: cover;
      vertical-align: top;
      -moz-box-sizing: border-box;
      -webkit-box-sizing: border-box;
      box-sizing: border-box;
      white-space: normal;
    }

    .csslider>ul>li.scrollable {
      overflow-y: scroll;
    }

    .csslider>.navigation {
      position: absolute;
      bottom: -10px;
      left: 50%;
      z-index: 10;
      margin-bottom: -10px;
      font-size: 0;
      line-height: 0;
      text-align: center;
      -webkit-touch-callout: none;
      -webkit-user-select: none;
      -khtml-user-select: none;
      -moz-user-select: none;
      -ms-user-select: none;
      user-select: none;
    }

    .csslider>.navigation>div {
      margin-left: -100%;
    }

    .csslider>.navigation label {
      position: relative;
      display: inline-block;
      cursor: pointer;
      border-radius: 50%;
      margin: 0 2px;
      padding: 5px;
      background: #d1d1d1;
    }

    .csslider>.navigation label:hover:after {
      opacity: 1;
    }

    .csslider>.navigation label:after {
      content: '';
      position: absolute;
      left: 50%;
      top: 50%;
      margin-left: -3px;
      margin-top: -3px;
      background: #0097ef;
      border-radius: 50%;
      padding: 3px;
      opacity: 0;
    }

    .csslider>.arrows {
      -webkit-touch-callout: none;
      -webkit-user-select: none;
      -khtml-user-select: none;
      -moz-user-select: none;
      -ms-user-select: none;
      user-select: none;
    }

    .csslider.inside .navigation {
      bottom: 10px;
      margin-bottom: 10px;
    }

    .csslider.inside .navigation label {
      border: 1px solid #7e7e7e;
    }

    .csslider>input:nth-of-type(1):checked~.navigation label:nth-of-type(1):after,
    .csslider>input:nth-of-type(2):checked~.navigation label:nth-of-type(2):after,
    .csslider>input:nth-of-type(3):checked~.navigation label:nth-of-type(3):after,
    .csslider>input:nth-of-type(4):checked~.navigation label:nth-of-type(4):after,
    .csslider>input:nth-of-type(5):checked~.navigation label:nth-of-type(5):after,
    .csslider>input:nth-of-type(6):checked~.navigation label:nth-of-type(6):after,
    .csslider>input:nth-of-type(7):checked~.navigation label:nth-of-type(7):after,
    .csslider>input:nth-of-type(8):checked~.navigation label:nth-of-type(8):after,
    .csslider>input:nth-of-type(9):checked~.navigation label:nth-of-type(9):after,
    .csslider>input:nth-of-type(10):checked~.navigation label:nth-of-type(10):after,
    .csslider>input:nth-of-type(11):checked~.navigation label:nth-of-type(11):after {
      opacity: 1;
    }

    .csslider>.arrows {
      position: absolute;
      left: -31px;
      top: 50%;
      width: 100%;
      height: 26px;
      padding: 0 31px;
      z-index: 0;
      -moz-box-sizing: content-box;
      -webkit-box-sizing: content-box;
      box-sizing: content-box;
    }

    .csslider>.arrows label {
      display: none;
      position: absolute;
      top: -50%;
      padding: 13px;
      box-shadow: inset 2px -2px 0 1px #d1d1d1;
      cursor: pointer;
      -moz-transition: .15s;
      -o-transition: .15s;
      -webkit-transition: .15s;
      transition: .15s;
    }

    .csslider>.arrows label:hover {
      box-shadow: inset 3px -3px 0 2px #0097ef;
      margin: 0 0px;
    }

    .csslider>.arrows label:before {
      content: '';
      position: absolute;
      top: -100%;
      left: -100%;
      height: 300%;
      width: 300%;
    }

    .csslider.infinity>input:first-of-type:checked~.arrows label:last-of-type,
    .csslider>input:nth-of-type(1):checked~.arrows label:nth-of-type(0),
    .csslider>input:nth-of-type(2):checked~.arrows label:nth-of-type(1),
    .csslider>input:nth-of-type(3):checked~.arrows label:nth-of-type(2),
    .csslider>input:nth-of-type(4):checked~.arrows label:nth-of-type(3),
    .csslider>input:nth-of-type(5):checked~.arrows label:nth-of-type(4),
    .csslider>input:nth-of-type(6):checked~.arrows label:nth-of-type(5),
    .csslider>input:nth-of-type(7):checked~.arrows label:nth-of-type(6),
    .csslider>input:nth-of-type(8):checked~.arrows label:nth-of-type(7),
    .csslider>input:nth-of-type(9):checked~.arrows label:nth-of-type(8),
    .csslider>input:nth-of-type(10):checked~.arrows label:nth-of-type(9),
    .csslider>input:nth-of-type(11):checked~.arrows label:nth-of-type(10) {
      display: block;
      left: 0;
      -moz-transform: rotate(45deg);
      -ms-transform: rotate(45deg);
      -o-transform: rotate(45deg);
      -webkit-transform: rotate(45deg);
      transform: rotate(45deg);
    }

    .csslider.infinity>input:last-of-type:checked~.arrows label:first-of-type,
    .csslider>input:nth-of-type(1):checked~.arrows label:nth-of-type(2),
    .csslider>input:nth-of-type(2):checked~.arrows label:nth-of-type(3),
    .csslider>input:nth-of-type(3):checked~.arrows label:nth-of-type(4),
    .csslider>input:nth-of-type(4):checked~.arrows label:nth-of-type(5),
    .csslider>input:nth-of-type(5):checked~.arrows label:nth-of-type(6),
    .csslider>input:nth-of-type(6):checked~.arrows label:nth-of-type(7),
    .csslider>input:nth-of-type(7):checked~.arrows label:nth-of-type(8),
    .csslider>input:nth-of-type(8):checked~.arrows label:nth-of-type(9),
    .csslider>input:nth-of-type(9):checked~.arrows label:nth-of-type(10),
    .csslider>input:nth-of-type(10):checked~.arrows label:nth-of-type(11),
    .csslider>input:nth-of-type(11):checked~.arrows label:nth-of-type(12) {
      display: block;
      right: 0;
      -moz-transform: rotate(225deg);
      -ms-transform: rotate(225deg);
      -o-transform: rotate(225deg);
      -webkit-transform: rotate(225deg);
      transform: rotate(225deg);
    }

    /*#region MODULES */
    /*#endregion */
  </style>
  <style>
    .csslider .navigation label {
      background: #B1B1B1;
    }

    .csslider .arrows label {
      border-left-color: #B1B1B1;
      border-right-color: #B1B1B1;
    }

    .csslider.inside .navigation label {
      border: 1px solid #FFF;
    }

    @import url(http://fonts.googleapis.com/css?family=Raleway:400,700|Lato);



    ::-webkit-scrollbar {
      width: 2px;
      background: rgba(255, 255, 255, 0.1);
    }

    ::-webkit-scrollbar-track {
      background: none;
    }

    ::-webkit-scrollbar-thumb {
      background: rgba(0, 94, 168, 0.6);
    }





    #slider1 {
      margin: 20px;
      font-family: 'Lato';
    }

    #slider1>ul>li:nth-of-type(3) {
      background: url(./themes/fruit.jpg);
    }

    #slider1>input:nth-of-type(3):checked~ul #bg {
      width: 80%;
      padding: 22px;
      -moz-transition: .5s .5s;
      -o-transition: .5s .5s;
      -webkit-transition: .5s .5s;
      transition: .5s .5s;
    }

    #slider1>input:nth-of-type(3):checked~ul #bg div {
      -moz-transform: translate(0);
      -ms-transform: translate(0);
      -o-transform: translate(0);
      -webkit-transform: translate(0);
      transform: translate(0);
      -moz-transition: .5s .9s;
      -o-transition: .5s .9s;
      -webkit-transition: .5s .9s;
      transition: .5s .9s;
    }

    #bg {
      color: #000;
      padding: 22px 0;
      position: absolute;
      left: 0;
      top: 16%;
      height: 20%;
      width: 0;
      z-index: 10;
      overflow: hidden;
    }

    #bg:before {
      content: '';
      position: absolute;
      left: -1px;
      top: 1px;
      height: 100%;
      width: 100%;
      z-index: -1;
      background: url(./themes/fruit.jpg) 1px 23%;
      -webkit-filter: blur(7px);
    }

    #bg:after {
      content: '';
      position: absolute;
      left: 0;
      top: 0;
      height: 100%;
      width: 100%;
      z-index: 20;
      background: rgba(0, 0, 0, 0.35);
      pointer-events: none;
    }

    #bg div {
      -moz-transform: translate(120%);
      -ms-transform: translate(120%);
      -o-transform: translate(120%);
      -webkit-transform: translate(120%);
      transform: translate(120%);
    }

    .scrollable p {
      padding: 30px;
      text-align: justify;
      line-height: 140%;
      font-size: 120%;
    }
  </style>




</head>

<body>

  <link rel="preconnect" href="https://fonts.gstatic.com" />
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@40a0;500;600;700&display=swap" rel="stylesheet" />
  <link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/devicons/devicon@v2.14.0/devicon.min.css" />
  <script src="https://kit.fontawesome.com/fa62c117c7.js" crossorigin="anonymous"></script>
  <header id="top">
    <a class="icon-border header-title" href="#">FL</a>
    <nav>
      <ul>
        <li>
          <a href="#project" class="link">Projects</a>
        </li>
        <li>
          <a href="#techstack" class="link">Tech Stack</a>
        </li>
        <li>
          <a href="#contact" class="link">Contact</a>
        </li>
        <li>
          <a href="#team" class="link">My Teams</a>
        </li>
      </ul>

      &nbsp; &nbsp;

      <label id="switch" class="switch">
        <input type="checkbox" onchange="toggleTheme()" id="slider">
        <span class="slider round"></span>
      </label>
      <!--<button aria-label="Toggle theme">
                  <i aria-hidden="true" class="icon-normal fas fa-moon"></i>
              </button>-->
      <!--<button aria-label="Toggle navbar"><i aria-hidden="true" class="icon-normal fas fa-bars"></i></button>-->
    </nav>
  </header>

  <div class="hero">
    <h1>
      Hi. I am
      <span class="hero-name">First</span>
      <span class="hero-name">Last</span>
    </h1>

    <div class="hero-about">
      <p class="para1">
        I am a <b><em>Salesforce developer</em></b>. I enjoy writing clean code, building
        beautiful Components as per the needs, and Finding the best solutions
        for your CRM implementations.
      </p>

      <a class="resume" href="https://1drv.ms/b/s!AiDyzNrKt_XHoFaofFgZV_mo3Vn2?e=lrL92a">
        <span class="btn">Resume</span>
      </a>
    </div>
  </div>

  <br/>

  <br/>

  <br/>

  <br/>

  <section id="project" class="project">
    <h2 class="section-title">Projects</h2>

    <div class="project-container">

      <img src="project1.png" alt="project image" height="250" width="450" />

      <div class="project-content">
        <h3>Order Management System</h3>
        <p class="para1">
          This Order Management System is a Salesforce application and the Envirnment which is meant to facilitate the
          creation and approval of orders generated by the client's firm
          the firm's order handeling team comprises employees in sales, bussiness and support roles.
        </p>

        <ul class="project-skill">
          <li>Apex</li>
          <li>Triggers</li>
          <li>LWC</li>
        </ul>

        <!--<ul class="project-link">
          <li>
              <a href="#">link</a>
          </li>
        </ul>-->
      </div>
    </div>

    <!-- <div class="project-container">
              <img src="./assets/images/startpage.png" alt="startpage" />
              <div class="project-content">
                  <h3>Startpage</h3>
                  <p>A minimal startpage for Firefox.</p>
                  <ul class="project-skill">
                      <li>HTML</li>
                      <li>CSS</li>
                      <li>JavaScript</li>
                  </ul>
                  <ul class="project-link">
                      <li>
                          <a href="#" aria-label="Source code" target="_blank"
                              title="source code" rel="noopener"><i class="icon-border fas fa-code"></i></a>
                      </li>
                      <li>
                          <a href="#" aria-label="Preview" target="_blank"
                              title="preview" rel="noopener"><i aria-hidden="true"
                                  class="icon-border fas fa-external-link-alt"></i></a>
                      </li>
                  </ul>
              </div>
          </div> -->


    <div class="project-container">

      <img src="project1.png" alt="project image" height="250" width="450" />

      <div class="project-content">
        <h3>Consultancy Project</h3>
        <p class="para1">
          This consultancy is focused on maintaining the candidate data with their skill set
          so that if some company approaches the consultancy with the ask for a particular skill set
          they can readily provide them with the resource.
        </p>

        <ul class="project-skill">
          <li>Apex</li>
          <li>Triggers</li>
          <li>LWC</li>
        </ul>
      </div>
    </div>

    <br />

    <br />

    <h2 class="section-title" id="techstack">Tech Stack</h2>
    <div class="stack-container">
      <div class="tech-container">
        <i class="devicon-html5-plain colored"></i>
        HTML
      </div>
      <div class="tech-container">
        <i class="devicon-css3-plain colored"></i>
        CSS
      </div>
      <div class="tech-container">
        <i class="devicon-javascript-plain colored"></i>
        JavaScript
      </div>
      <div class="tech-container">

        <i class="devicon-php-plain colored"></i>

        php
      </div>
      <div class="tech-container">
        <i class="devicon-salesforce-plain colored"></i>
        Salesforce
      </div>
      <div class="tech-container">
        <i class="devicon-Github-plain colored"></i>
        Github
      </div>
      <div class="tech-container">
        <i class="devicon-c-plain colored"></i>
        C
      </div>

      <div class="tech-container">

        <i class="devicon-java-plain-wordmark colored"></i>

        Java
      </div>
      <div class="tech-container">

        <i class="devicon-mysql-plain colored"></i>

        Mysql
      </div>

      <div class="tech-container">
        <i class="devicon-oracle-plain"></i>
        oracle
      </div>

    </div>

    <br />

    <br />

    <br />

    <br />


    <h2 class="section-title" id="team">My Team</h2>
    <!-- team section start -->
    <section class="teams" id="teams" style="margin-top: 0px !important;">
      <div class="max-width" style="    width: 860px !important; padding: 0px !important; ">





        <div id="slider1" class="csslider infinity inside">
          <input type="radio" name="slides" id="slides_1" checked />
          <input type="radio" name="slides" id="slides_2" />
          <input type="radio" name="slides" id="slides_3" />
          <input type="radio" name="slides" id="slides_4" />
          <ul>
            <li>
              <div class="carousel owl-carousel">
                <div class="card">
                  <div class="box">
                    <img src="https://i.ibb.co/fN75gWz/image-2022-07-26-202207222.png" alt="image-2022-07-26-202207222"
                      border="0">
                    <div class="text">Someone name</div>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Lorem ipsum dolor sit amet consectetur adipisicing elit. Sit repudiandae veniam eum atque explicabo quod, sunt consequatur expedita? Quos nulla doloribus quod recusandae repudiandae, eligendi doloremque inventore commodi incidunt magnam?</p>
                  </div>
                </div>
              </div>

            </li>
            <li>
              <div class="carousel owl-carousel">
                <div class="card">
                  <div class="box">
                    <img src="https://i.ibb.co/fN75gWz/image-2022-07-26-202207222.png" alt="image-2022-07-26-202207222"
                      border="0">
                    <div class="text">Someone name</div>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
                  </div>
                </div>
              </div>
            </li>
            <li>
              <div class="carousel owl-carousel">
                <div class="card">
                  <div class="box">
                    <img src="https://i.ibb.co/fN75gWz/image-2022-07-26-202207222.png" alt="image-2022-07-26-202207222"
                      border="0">
                    <div class="text">Someone name</div>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
                  </div>
                </div>
              </div>
            </li>
            <li>
              <div class="carousel owl-carousel">
                <div class="card">
                  <div class="box">
                    <img src="https://i.ibb.co/fN75gWz/image-2022-07-26-202207222.png" alt="image-2022-07-26-202207222"
                      border="0">
                    <div class="text">Someone name</div>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
                  </div>
                </div>
              </div>
            </li>
          </ul>
          <div class="arrows">
            <label for="slides_1"></label>
            <label for="slides_2"></label>
            <label for="slides_3"></label>
            <label for="slides_4"></label>
          </div>
          <div class="navigation">
            <div>
              <label for="slides_1"></label>
              <label for="slides_2"></label>
              <label for="slides_3"></label>
              <label for="slides_4"></label>
            </div>
          </div>
        </div>


      </section>


      <br/>

      <br/>


    <script>
      $(document).ready(function () {
        $(window).scroll(function () {
          // sticky navbar on scroll script
          if (this.scrollY > 20) {
            $('.navbar').addClass("sticky");
          } else {
            $('.navbar').removeClass("sticky");
          }

          // scroll-up button show/hide script
          if (this.scrollY > 500) {
            $('.scroll-up-btn').addClass("show");
          } else {
            $('.scroll-up-btn').removeClass("show");
          }
        });

        // slide-up script
        $('.scroll-up-btn').click(function () {
          $('html').animate({ scrollTop: 0 });
          // removing smooth scroll on slide-up button click
          $('html').css("scrollBehavior", "auto");
        });

        $('.navbar .menu li a').click(function () {
          // applying again smooth scroll on menu items click
          $('html').css("scrollBehavior", "smooth");
        });

        // toggle menu/navbar script
        $('.menu-btn').click(function () {
          $('.navbar .menu').toggleClass("active");
          $('.menu-btn i').toggleClass("active");
        });

        // typing text animation script
        var typed = new Typed(".typing", {
          strings: ["Developer", "Designer", "Freelancer"],
          typeSpeed: 100,
          backSpeed: 60,
          loop: true
        });

        var typed = new Typed(".typing-2", {
          strings: ["Developer", "Designer", "Freelancer"],
          typeSpeed: 100,
          backSpeed: 60,
          loop: true
        });

        // owl carousel script
        $('.carousel').owlCarousel({
          margin: 20,
          loop: true,
          autoplay: true,
          autoplayTimeOut: 2000,
          autoplayHoverPause: true,
          responsive: {
            0: {
              items: 1,
              nav: false
            },
            600: {
              items: 2,
              nav: false
            },
            1000: {
              items: 3,
              nav: false
            }
          }
        });
      });
      Footer

    </script>


    <section id="contact" class="contact">
      <h2 class="section-title">Get in touch</h2>

      <br />

      <div class="max-width">
        <div class="content-content">
          <div class="column left">
            <div class="text">
              About
            </div>
            <p>Lorem ipsum dicta repellendus ab unde et a? Ullam quae recusandae dolor voluptatem rerum qui
              aspernatur veritatis.</p>
            <div class="icons">
              <div class="row">
                <i class="fas fa-user"></i>
                <div class="info">
                  <div class="head">Name</div>
                  <div class="sub-title">My Name</div>
                </div>
              </div>
              <div class="row">
                <i class="fas fa-map-marker-alt"></i>
                <div class="info">
                  <div class="head">Address</div>
                  <div class="sub-title">Ghaziabad, Utter Pradesh, India</div>
                </div>
              </div>
              <div class="row">
                <i class="fas fa-envelope"></i>
                <div class="info">
                  <div class="head">Email</div>
                  <div class="sub-title">myEmail@gmail.com</div>
                </div>
              </div>
            </div>
          </div>

          <div class="column right">
            <div class="text">
              Message me
            </div>
            <form action="$">
              <div class="fileds">
                <div class="field name">
                  <input type="text" placeholder="Name" required>
                </div>

                <div class="field email">
                  <input type="email" placeholder="Email" required>
                </div>
              </div>
              <div class="field">
                <input type="text" placeholder="Subject" required>
              </div>
              <div class="field textarea">
                <textarea cols="30" rows="10" placeholder="Describe project.." required></textarea>
              </div>
              <div class="button">
                <button type="submit">Send Message</button>
              </div>
            </form>
          </div>

        </div>

        <br />

        <br />


        <ul>
          <li>
            <a href="mailto:enterMail@gmail.com">
              <span class="btn">
                <i aria-hidden="true" class="fas icon fa-envelope"></i>Email
              </span>
            </a>
          </li>

          <li>
            <a href="https://github.com/username" aria-label="Github">
              <span class="btn">
                <i aria-hidden="true" class="fab icon fa-github"></i>
                Github
              </span>
            </a>
          </li>

          <li>
            <a href="https://www.linkedin.com/in/username/" aria-label="Linkedin">
              <span class="btn">
                <i aria-hidden="true" class="fab icon fa-linkedin"></i>
                Linkedin
              </span>
            </a>
          </li>

          <li>
            <a href="https://www.instagram.com/username/" aria-label="Instagram">
              <span class="btn">
                <i aria-hidden="true" class="fab icon fa-instagram"></i>
                Instagram
              </span>
            </a>
          </li>
        </ul>
      </div>


    </section>


    <footer>
      <small>&copy; 2020-2022 my name</small>
    </footer>

    <div class="scroll-container">
      <div aria-label="Scroll up" class="scroll-up">
        <a href="#top">
          <i aria-hidden="true" class="fas fa-arrow-up"></i>
        </a>
      </div>
    </div>

    <!-- https://codepen.io/vats147/pen/PoRJqvE -->


</body>
<script>

  const btnHamburger = document.querySelector(".fa-bars");
  const btnTheme = document.querySelector(".fa-moon");

  btnHamburger.addEventListener("click", displayList);
  btnTheme.addEventListener("click", toggleTheme);
  document.addEventListener("scroll", scroll.scrollUp);

  const getBodyClass = localStorage.getItem("class-body-theme");
  const getBtnClass = localStorage.getItem("class-btn-theme");

  addThemeClass(getBodyClass, getBtnClass);

</script>
<script>
  // function to set a given theme/color-scheme
  function setTheme(themeName) {
    localStorage.setItem('theme', themeName);
    document.documentElement.className = themeName;
  }

  // function to toggle between dark theme and light theme
  function toggleTheme() {
    if (localStorage.getItem('theme') === 'theme-dark') {
      setTheme('theme-light');
    } else {
      setTheme('theme-dark');
    }
  }

  // initial theme setup
  (function () {
    if (localStorage.getItem('theme') === 'theme-dark') {
      setTheme('theme-dark');
      document.getElementById('slider').checked = false;
    } else {
      setTheme('theme-light');
      document.getElementById('slider').checked = true;
    }
  })();

</script>

<script>

  $(document).ready(function () {
    $(window).scroll(function () {
      // sticky navbar on scroll script
      if (this.scrollY > 20) {
        $('.navbar').addClass("sticky");
      } else {
        $('.navbar').removeClass("sticky");
      }

      // scroll-up button show/hide script
      if (this.scrollY > 500) {
        $('.scroll-up-btn').addClass("show");
      } else {
        $('.scroll-up-btn').removeClass("show");
      }
    });

    // slide-up script
    $('.scroll-up-btn').click(function () {
      $('html').animate({ scrollTop: 0 });
      // removing smooth scroll on slide-up button click
      $('html').css("scrollBehavior", "auto");
    });

    $('.navbar .menu li a').click(function () {
      // applying again smooth scroll on menu items click
      $('html').css("scrollBehavior", "smooth");
    });

    // toggle menu/navbar script
    $('.menu-btn').click(function () {
      $('.navbar .menu').toggleClass("active");
      $('.menu-btn i').toggleClass("active");
    });

    // typing text animation script
    var typed = new Typed(".typing", {
      strings: ["Developer", "Designer", "Freelancer"],
      typeSpeed: 100,
      backSpeed: 60,
      loop: true
    });

    var typed = new Typed(".typing-2", {
      strings: ["Developer", "Designer", "Freelancer"],
      typeSpeed: 100,
      backSpeed: 60,
      loop: true
    });



    // owl carousel script
    $('.carousel').owlCarousel({
      margin: 20,
      loop: true,
      autoplay: true,
      autoplayTimeOut: 2000,
      autoplayHoverPause: true,
      responsive: {
        0: {
          items: 1,
          nav: false
        },
        600: {
          items: 2,
          nav: false
        },
        1000: {
          items: 3,
          nav: false
        }
      }
    });
  });
</script>

</html>
```

