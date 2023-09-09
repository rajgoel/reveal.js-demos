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

===

### Hosting a seminar

Everyone knowing the password of the seminar can start and host a seminar.

You can enter the password and an optional (nick)name of your choice in the <i class="fa fa-rss"></i> Broadcast section of the menu that you can reach by clicking the <i class="fa fa-bars"></i> button in the lower left corner. To host a seminar simply click the 'Start' button. 


For this presentation, the password is `123456`.

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

This requires the `poll` plugin.

===

### Questions & Answers

This requires the `questions` plugin.


