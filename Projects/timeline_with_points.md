### image 

![image](https://user-images.githubusercontent.com/63545175/183058408-7ac744a3-5e68-46eb-8d32-3835d82c06ad.png)



### code 

```html
<html>
  <head>
    <style>
      body {
        font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
      }

      #experience-timeline {
        margin: 30px auto 0 auto;
        position: relative;
        max-width: 1000px;
      }
      #experience-timeline:before {
        position: absolute;
        content: "";
        top: 0;
        bottom: 0;
        left: 302px;
        right: auto;
        height: 100%;
        width: 4px;
        background: #16f087;
        z-index: 0;
      }
      #experience-timeline:after {
        position: absolute;
        content: "";
        width: 4px;
        height: 40px;
        background: linear-gradient(to bottom, #16f04d, rgba(22, 136, 240, 0));
        top: 100%;
        left: 302px;
      }

      .notch {
        display: block;
        height: 20px;
        width: 20px;
        background-color: inherit;
        border: inherit;
        position: absolute;
        top: 20px;
        left: 342px;
        clip-path: polygon(0% 0%, 100% 100%, 0% 100%);
        transform: rotate(45deg);
        border-radius: 0 0 0 0.25em;
      }

      .timeline-content {
        margin-left: 350px;
        background: rgb(215, 215, 215);
        padding: 15px;
        border-radius: 10px;
        text-align: left;
      }
      .timeline-content h3 {
        font-size: 1.5em;
        font-weight: 500;
        color: #000000;
        display: inline-block;
        margin: 0;
      }
      .timeline-content h4 {
        font-size: 1.2em;
        font-weight: 400;
        font-style: italic;
        color: #797979;
        margin: 0 0 15px 0;
      }
      .timeline-content p {
        color: #dedede;
        font-size: 0.9em;
        margin: 0;
      }

      .timeline-point {
        position: relative;
        display: block;
        margin-bottom: 30px;
      }
      .timeline-icon {
        position: relative;
        color: #dedede;
        width: 30px;
        height: 30px;
        background: #095963;
        border-radius: 50%;
        float: left;
        z-index: 99;
        margin-left: 287px;
        margin-top: 6px;
        box-shadow: 3px 6px 9px #5c5c5c;
        padding: 2px 2px 2px 2px;
        text-align: center;
      }

      .timeline-date {
        width: 260px;
        text-align: right;
        position: absolute;
        left: 0;
        top: 10px;
        font-weight: 400;
        color: #383838;
      }

      @media only screen and (max-width: 800px) {
        #experience-timeline:before {
          top: 18px;
          left: 25px;
        }
        #experience-timeline:after {
          left: 25px;
        }
        .timeline-date {
          width: auto;
          text-align: left;
          position: relative;
          margin-bottom: 15px;
          display: block;
          margin-left: 70px;
        }
        .timeline-icon {
          margin-left: 10px;
          top: 40px;
        }
        .timeline-content {
          margin-left: 70px;
        }
        .notch {
          top: 60px;
          left: 62px;
        }
      }
    </style>
  </head>

  <body>
    <h1 style="text-align: center">Timeline with points</h1>

    <br />

    <div id="experience-timeline">
      <div class="timeline-point">
        <div class="timeline-icon">💼</div>
        <div class="timeline-block">
          <span class="timeline-date">July 2021 – present</span>
          <div class="shadow timeline-content">
            <div class="notch"></div>

            <h3>Title</h3>
            <h4>sub title</h4>
            Lorem ipsum, dolor sit amet consectetur adipisicing elit.
            <ul>
              <li>
                Lorem ipsum dolor sit amet consectetur, adipisicing elit. Quidem
                eaque quos ab alias modi, repellendus.
              </li>
              <li>
                Lorem ipsum dolor sit amet consectetur, adipisicing elit. Quidem
                eaque quos ab alias modi, repellendus nulla eos, odit.
              </li>
              <li>
                Lorem ipsum dolor sit amet consectetur, adipisicing elit. Quidem
                eaque quos ab alias modi, repellendus nulla eos, odit quae,
                itaque voluptatum.
              </li>
              <li>
                Lorem ipsum dolor sit amet consectetur, adipisicing elit. Quidem
                eaque quos ab alias modi, repellend.
              </li>
            </ul>
          </div>
        </div>
      </div>

      <div class="timeline-point">
        <div class="timeline-icon">💼</div>
        <div class="timeline-block">
          <span class="timeline-date">July 2020 – July 2021</span>
          <div class="shadow timeline-content art-a art-card">
            <div class="notch"></div>

            <h3>Title</h3>
            <h4>sub title</h4>
            <ul>
              <li>
                Lorem ipsum, dolor sit amet consectetur adipisicing elit. Atque
                modi odio cumque laboriosam, impe.
              </li>
              <li>
                Lorem ipsum, dolor sit amet consectetur adipisicing elit. Atque
                modi odio cumque laboriosam, impedit pariatur alias autem rem
                doloremque reiciendis aliquam teorum.
              </li>
              <li>Lorem ipsum, dolor sit amet conseorum.</li>
            </ul>
          </div>
        </div>
      </div>
      <div class="timeline-point">
        <div class="timeline-icon">🎓</div>
        <div class="timeline-block">
          <span class="timeline-date">July 2019 – July 2020</span>
          <div class="timeline-content art-a art-card">
            <div class="notch"></div>

            <h3>title</h3>
            <h4>Sub title</h4>
            <ul>
              <li>
                Lorem ipsum dolor sit amet consectetur adipisicing elit.
                Consequuntur eos magni dolor saepe quae.
              </li>
              <li>
                Lorem ipsum dolor sit amet consectetur adipisicing elit.
                Consequuntur eos magni dolor sint minus, saepe quae.
              </li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </body>
</html>

```
