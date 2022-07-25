### Images
![image](https://user-images.githubusercontent.com/63545175/180811284-6ad14b95-44d6-4490-a03f-10ea5a5db28e.png)

![image](https://user-images.githubusercontent.com/63545175/180811189-28d49bd7-5f4e-49c9-8b9b-8a823b963353.png)



### code

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>BASIC CHAT APP</title>
    <link rel="manifest" href="manifest.json" />
    <script src="https://www.gstatic.com/firebasejs/7.21.0/firebase-app.js"></script>
    <script src="https://www.gstatic.com/firebasejs/7.21.0/firebase-auth.js"></script>
    <script src="https://www.gstatic.com/firebasejs/7.21.0/firebase-database.js"></script>

    <style>
      h6 {
        display: inline !important;
        font-weight: bold;
        font-style: italic;
      }

      .login-with-google-btn {
        transition: background-color 0.3s, box-shadow 0.3s;

        padding: 12px 16px 12px 42px;
        border: none;
        border-radius: 3px;
        box-shadow: 0 -1px 0 rgba(0, 0, 0, 0.04), 0 1px 1px rgba(0, 0, 0, 0.25);

        color: #757575;
        font-size: 14px;
        font-weight: 500;
        font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto,
          Oxygen, Ubuntu, Cantarell, "Fira Sans", "Droid Sans", "Helvetica Neue",
          sans-serif;

        background-image: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTgiIGhlaWdodD0iMTgiIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyI+PGcgZmlsbD0ibm9uZSIgZmlsbC1ydWxlPSJldmVub2RkIj48cGF0aCBkPSJNMTcuNiA5LjJsLS4xLTEuOEg5djMuNGg0LjhDMTMuNiAxMiAxMyAxMyAxMiAxMy42djIuMmgzYTguOCA4LjggMCAwIDAgMi42LTYuNnoiIGZpbGw9IiM0Mjg1RjQiIGZpbGwtcnVsZT0ibm9uemVybyIvPjxwYXRoIGQ9Ik05IDE4YzIuNCAwIDQuNS0uOCA2LTIuMmwtMy0yLjJhNS40IDUuNCAwIDAgMS04LTIuOUgxVjEzYTkgOSAwIDAgMCA4IDV6IiBmaWxsPSIjMzRBODUzIiBmaWxsLXJ1bGU9Im5vbnplcm8iLz48cGF0aCBkPSJNNCAxMC43YTUuNCA1LjQgMCAwIDEgMC0zLjRWNUgxYTkgOSAwIDAgMCAwIDhsMy0yLjN6IiBmaWxsPSIjRkJCQzA1IiBmaWxsLXJ1bGU9Im5vbnplcm8iLz48cGF0aCBkPSJNOSAzLjZjMS4zIDAgMi41LjQgMy40IDEuM0wxNSAyLjNBOSA5IDAgMCAwIDEgNWwzIDIuNGE1LjQgNS40IDAgMCAxIDUtMy43eiIgZmlsbD0iI0VBNDMzNSIgZmlsbC1ydWxlPSJub256ZXJvIi8+PHBhdGggZD0iTTAgMGgxOHYxOEgweiIvPjwvZz48L3N2Zz4=);
        background-color: white;
        background-repeat: no-repeat;
        background-position: 12px 11px;
      }

      .login-with-google-btn:hover {
        box-shadow: 0 -1px 0 rgba(0, 0, 0, 0.04), 0 2px 4px rgba(0, 0, 0, 0.25);
      }

      .login-with-google-btn:active {
        background-color: #eeeeee;
      }

      .login-with-google-btn:focus {
        outline: none;
        box-shadow: 0 -1px 0 rgba(0, 0, 0, 0.04), 0 2px 4px rgba(0, 0, 0, 0.25),
          0 0 0 3px #c8dafc;
      }

      body {
        font: 12px arial;
        color: #222;
        text-align: center;
        padding: 35px;
      }

      form,
      p,
      span {
        margin: 0;
        padding: 0;
      }

      input {
        font: 12px arial;
      }

      a {
        color: #0000ff;
        text-decoration: none;
      }

      a:hover {
        text-decoration: underline;
      }

      #wrapper,
      #loginform {
        margin: 0 auto;
        padding-bottom: 25px;
        background: #bcc0c0;
        width: 514px;
        border: 6px solid #ebebeb;
        border-radius: 6px;
      }

      #loginform {
        padding-top: 18px;
      }

      #loginform p {
        margin: 5px;
      }

      #chatbox {
        text-align: left;
        margin: 0 auto;
        margin-bottom: 5px;
        padding: 10px;
        background: #fff;
        height: 270px;
        width: 460px;
        border: 1px solid #ebebeb;
        overflow: auto;
        border-radius: 5px;
      }

      .usermsg {
        width: 390px;
        padding: 10px;
        border: none;
        background: #fff;
        resize: none;
        border-radius: 5px;
      }

      .send-msg-btn {
        background-color: rgb(35, 140, 182);
        color: white;
        padding: 11px 15px;
        border: none;
        cursor: pointer;
        width: 13%;
        margin-bottom: 10px;
        opacity: 0.8;
        border-radius: 5px;
      }

      .send-msg-btn:hover {
        background-color: rgb(18, 61, 79);
        color: white;
      }
      .error {
        color: #ff0000;
      }

      #menu {
        padding: 12.5px 25px 12.5px 25px;
      }

      .welcome {
        float: left;
        font-size: 18px;
        color: teal;
      }

      .login-google-btn {
        float: center;
        background-color: rgb(35, 140, 182);
        color: white;
        padding: 10px 14px;
        border: none;
        cursor: pointer;
        width: 18%;
        margin-bottom: 10px;
        opacity: 0.8;
        border-radius: 5px;
        font-size: 10px;
        margin-right: 2px;
      }
      .login-google-btn:hover {
        background-color: rgb(110, 196, 230);
        color: white;
      }

      .msgln {
        margin: 0 0 2px 0;
      }

      li {
        display: list-item;
        text-align: -webkit-match-parent;
        font-size: 16px;
      }

      @media screen and (max-width: 518px) {
      }
    </style>

    <script>
      // Your web app's Firebase configuration
      // For Firebase JS SDK v7.20.0 and later, measurementId is optional
      var firebaseConfig = {
        apiKey: " ",
        authDomain: " ",
        databaseURL: " ",
        projectId: " ",
        storageBucket: " ",
        messagingSenderId: " ",
        appId: " ",
        measurementId: " ",
      };

      // Initialize Firebase
      firebase.initializeApp(firebaseConfig);
    </script>
  </head>

  <body>

    <script>
            let userName;
    let userPicture;

    const google_login = () => {
      var provider = new firebase.auth.GoogleAuthProvider();

      firebase
        .auth()
        .signInWithPopup(provider)
        .then(function (result) {
          var token = result.credential.accessToken;
          let user = result.user;

          userName = user.displayName;

          userPicture = user.photoURL;

          //console.log("user ===> ", user);

          document.getElementById("login-box").style.display = "none";
          document.getElementById("msg-box").style.display = "block";
        })
        .catch(function (error) {
          console.log(error.message);
        });
    };

    const sendMessage = () => {
      let message = document.getElementById("message").value;
      firebase.database().ref("messages").push().set({
        sender: userName,
        message: message,
        picture: userPicture,
      });
      let message1 = document.getElementById("message");
      message1.value = "";
      return false;
    };

    </script>
    <div id="wrapper">
      <div id="login-box" class="align-center" style="display: block">
        <button
          type="submit"
          class="login-with-google-btn"
          onclick="google_login()"
        >
          Log in with Google
        </button>
      </div>

      <div id="msg-box" style="display: none">
        <div id="chatbox" style="margin-top: 20px !important">
          <ul id="messages" style="list-style-type: none; padding: 10px"></ul>
        </div>
        <!--  
        <form onsubmit="return sendMessage();">
            <input name="usermsg" type="text" id="usermsg" size="63" placeholder="Text Message" />
            <button id="button" class="button">Send</button>
        </form> -->

        <form onsubmit="return sendMessage();">
          <input
            type="text"
            id="message"
            class="usermsg"
            size="63"
            placeholder="Text Message"
            autocomplete="off"
            onclick="scrollChat();"
          />
          <input type="submit" class="send-msg-btn" value="SEND" />
        </form>
        <!-- <ul id="messages"></ul> -->
      </div>
    </div>
      <script>
    userName = "NULL";
    // listen for incoming messages
    firebase
      .database()
      .ref("messages")
      .on("child_added", function (snapshot) {
        var html = "";
        // give each message a unique ID
        html += "<li id='message-" + snapshot.key + "'>";

        html +=
          "<img style='margin-top:15px !important; width:30px !important; height:30px !important; border-radius:50% !important;' src=" +
          snapshot.val().picture +
          "></img>" +
          "<h6>" +
          snapshot.val().sender +
          "</h6>  : <br/> <p style='margin-left:8px !important; background-color: #dcd6d6; border-radius: 0px 12px 12px 12px !important; padding:10px;'>" +
          snapshot.val().message +
          "</p>";
        html += "</li>";
        /*
        // show delete button if message is sent me
        if (snapshot.val().sender == userName) {
          html +=
            "<button data-id='" +
            snapshot.key +
            "' onclick='deleteMessage(this);'>";
          html += "Delete";
          html += "</button>";
        };
        */

        document.getElementById("messages").innerHTML += html;

      // auto scroll to bottom of chat box when new text is added
      var elem = document.getElementById("chatbox");
      elem.scrollTop = elem.scrollHeight;

      });
    function deleteMessage(self) {
      // get message ID
      var messageId = self.getAttribute("data-id");

      // delete message
      firebase.database().ref("messages").child(messageId).remove();
    }

    // attach listener for delete message
    firebase
      .database()
      .ref("messages")
      .on("child_removed", function (snapshot) {
        // remove message node
        document.getElementById("message-" + snapshot.key).innerHTML =
          "This message has been removed";
      });

    // auto scroll to bottom of chat box
    function scrollChat() {
      var elem = document.getElementById("chatbox");
      elem.scrollTop = elem.scrollHeight;
    };

  </script>


  </body>
</html>
```
