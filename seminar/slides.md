## Seminars with Reveal.js

The `seminar` plugin allows to add live broadcasting of slide changes, chalkboard drawings, online polls, and Q&As to a slide deck.

---

### Requirements

The `seminar` plugin requires a running socket.io server.
<span class="seminar disconnected">
This demo presentation is <span style="color:red;"><i class="fa-solid fa-square-rss"></i> not connected </span> to a running server.
</span>
<span class="seminar connected">
This demo presentation is <span style="color:darkgreen;"><i class="fa-solid fa-square-rss"></i> connected </span> to a running  server.
</span>

---

### Seminar server

The seminar server can be obtained here [here](https://github.com/rajgoel/seminar).

<iframe src="https://ghbtns.com/github-btn.html?user=rajgoel&repo=seminar&type=star&count=true&size=large" frameborder="0" scrolling="0" width="170" height="30" title="GitHub"></iframe>

To learn how to setup your own server please check the [documentation](https://github.com/rajgoel/reveal.js-plugins/tree/master/seminar).

---

### Local test installation

To test the seminar plugin locally simply [download](https://github.com/rajgoel/seminar) the seminar server and run

```
npm install
npm run start
```

When you open this demo presentation it will connect to the locally running seminar server.

---

### Online seminars

For online seminars, you need to install the seminar server on a publicly reachable server and change the plugin configuration accordingly.

---

### Generating a password hash

You can create a password hash on the page displayed when opening the URL of the seminar server in the browser.

===

### Hosting a seminar

Everyone knowing the password of the seminar can start and host a seminar.


---

### Start the demo seminar

To start this demo seminar, you can enter the password `123456` and an optional (nick)name of your choice in the <i class="fa fa-rss"></i> Broadcast section of the menu that you can reach by clicking the <i class="fa fa-bars"></i> button in the lower left corner. To host a seminar simply click the 'Start' button.

---

#### Multiple hosts

Multiple users can host a seminar together. When the last host leaves the seminar, the seminar is closed and all remaining attendees are kicked out.

---

Whenever a host advances to a new slide or fragment, the respective instruction is broadcasted to all connected attendees of the seminar and their presentation will automatically follow.

===

### Chalkboard

Chalkboard drawings and handwritten slide annotations of a host are broadcasted to all connected attendees of the seminar and their presentation will also display them.

This requires the `chalkboard` plugin.

===

### Online polls

With the `poll` plugin you can add instant polls like the one below to your slides.

<div class="poll" data-poll="approval">
	<button data-value="yes">Yes</button>
	<br>
	<button data-value="no">No</button>
	<br>
	<button data-value="maybe">Maybe</button>
	<br>
</div>
<p style="font-size:24px;color:gray;">Responses: <span class="voters" data-poll="approval">0</span></p>

---

The results of the poll can be displayed with help of the `chart` plugin.

<div style="position: relative;height:480px!important;width:1280px!important;">
<canvas data-chart="bar" data-poll="approval">
, Yes, No, Maybe
, 0, 0, 0
</canvas>
</div>


===

### Questions & Answers

With the `questions` plugin you can give attendees the possibility ask and upvote questions during the presentation.

To ask a question or view all questions simply click on the <i class="fa fa-comment"></i> button that is shown when the presentation is being hosted.
