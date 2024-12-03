```mermaid
sequenceDiagram
    participant browser
    participant server

    browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note
    activate server
    server-->>browser: 302 Redirect to /exampleapp/notes
    deactivate server

    browser->>server: GET https://studies.cs.helsinki.fi/exampleapp/notes
    activate server
    server-->>browser: HTML document
    deactivate server

    browser->>server: GET https://studies.cs.helsinki.fi/exampleapp/main.css
    activate server
    server-->>browser: the css file
    deactivate server

    browser->>server: GET https://studies.cs.helsinki.fi/exampleapp/main.js
    activate server
    server-->>browser: the JavaScript file
    deactivate server

    browser->>server: GET https://studies.cs.helsinki.fi/exampleapp/data.json
    activate server
    server-->>browser: [
  {
    "content": "Don't forget the potatoes",
    "date": "2024-12-02T12:59:37.947Z"
  },
  {
    "content": "Christ1oh1",
    "date": "2024-12-02T13:06:43.694Z"
  },
  {
    "content": "efer",
    "date": "2024-12-02T13:14:01.083Z"
  },
  {
    "content": "wewe",
    "date": "2024-12-02T13:18:50.884Z"
  },
  {
    "content": "weew",
    "date": "2024-12-02T13:19:13.285Z"
  },
  {
    "content": "Where is the milk",
    "date": "2024-12-02T13:27:21.138Z"
  },
  {
    "content": "wewe",
    "date": "2024-12-02T13:34:01.332Z"
  },
  {
    "content": "efer",
    "date": "2024-12-02T13:42:15.547Z"
  },
  {
    "content": "wewe",
    "date": "2024-12-02T13:42:27.603Z"
  },
  {
    "content": "efer",
    "date": "2024-12-02T13:48:07.587Z"
  },
  {
    "content": "gyatt",
    "date": "2024-12-02T14:07:56.733Z"
  },
  {
    "content": "te",
    "date": "2024-12-02T14:08:36.564Z"
  },
  {
    "content": "dfdsfsd",
    "date": "2024-12-02T14:09:31.677Z"
  },
  {
    "content": "ne w",
    "date": "2024-12-02T14:09:58.204Z"
  },
  {
    "content": "bingus",
    "date": "2024-12-02T14:30:26.931Z"
  },
  {
    "content": "hi",
    "date": "2024-12-02T14:38:29.613Z"
  },
  {
    "content": "oi",
    "date": "2024-12-02T14:38:43.251Z"
  },
  {
    "content": "oi",
    "date": "2024-12-02T14:39:07.868Z"
  },
  {
    "content": "ugh",
    "date": "2024-12-02T14:50:25.507Z"
  },
  {
    "content": "hello world",
    "date": "2024-12-02T14:56:35.623Z"
  },
  {
    "content": "a",
    "date": "2024-12-02T15:31:21.917Z"
  },
  {
    "content": "a",
    "date": "2024-12-02T15:35:05.098Z"
  },
  {
    "content": "spa",
    "date": "2024-12-02T15:35:32.778Z"
  },
  {
    "content": "new new new note",
    "date": "2024-12-02T16:25:59.437Z"
  },
  {
    "content": "hfdfghch",
    "date": "2024-12-02T16:35:06.899Z"
  },
  {
    "content": "TEST2",
    "date": "2024-12-02T16:52:14.328Z"
  },
  {
    "content": "TEST3",
    "date": "2024-12-02T16:53:51.007Z"
  },
  {
    "content": "TEST3",
    "date": "2024-12-02T16:54:24.471Z"
  },
  {
    "content": "TEST3",
    "date": "2024-12-02T16:58:59.459Z"
  },
  {
    "content": "TEST3",
    "date": "2024-12-02T16:59:04.476Z"
  },
  {
    "content": "TEST2",
    "date": "2024-12-02T17:00:44.094Z"
  },
  {
    "content": "Badumtss",
    "date": "2024-12-02T17:00:55.111Z"
  },
  {
    "content": "lol",
    "date": "2024-12-02T17:27:36.056Z"
  },
  {
    "content": "goo",
    "date": "2024-12-02T17:30:55.571Z"
  },
  {
    "content": "Hello, Moto!",
    "date": "2024-12-02T17:33:27.547Z"
  },
  {
    "content": "ratata",
    "date": "2024-12-02T17:34:31.626Z"
  },
  {
    "content": "aqaq",
    "date": "2024-12-02T17:35:42.992Z"
  },
  {
    "content": "Sending 2nd note",
    "date": "2024-12-02T17:35:50.390Z"
  },
  {
    "content": "",
    "date": "2024-12-02T17:44:47.424Z"
  },
  {
    "content": "another note",
    "date": "2024-12-02T17:47:56.017Z"
  },
  {
    "content": "",
    "date": "2024-12-02T18:05:23.358Z"
  },
  {
    "content": "",
    "date": "2024-12-02T18:14:30.300Z"
  },
  {
    "content": "et",
    "date": "2024-12-02T18:17:02.189Z"
  },
  {
    "content": "terve! olen amerikkalainen",
    "date": "2024-12-02T18:29:48.605Z"
  },
  {
    "content": "hey",
    "date": "2024-12-02T18:32:38.066Z"
  },
  {
    "content": "",
    "date": "2024-12-02T19:06:53.298Z"
  },
  {
    "content": "hei amerikkalainen",
    "date": "2024-12-02T19:40:54.784Z"
  },
  {
    "content": "",
    "date": "2024-12-02T19:52:22.169Z"
  },
  {
    "content": "lule",
    "date": "2024-12-02T20:06:37.370Z"
  },
  {
    "content": "y",
    "date": "2024-12-02T20:39:42.579Z"
  },
  {
    "content": "878",
    "date": "2024-12-02T21:12:51.626Z"
  },
  {
    "content": "",
    "date": "2024-12-02T22:30:25.142Z"
  },
  {
    "content": "hello",
    "date": "2024-12-02T22:36:31.688Z"
  },
  {
    "content": ":V",
    "date": "2024-12-02T23:27:23.518Z"
  },
  {
    "content": "qwerty",
    "date": "2024-12-03T00:07:54.764Z"
  },
  {
    "content": "",
    "date": "2024-12-03T02:55:22.755Z"
  },
  {
    "content": "",
    "date": "2024-12-03T02:55:22.755Z"
  },
  {
    "content": "dfdfg",
    "date": "2024-12-03T02:57:36.283Z"
  },
  {
    "content": "HelloV0.1",
    "date": "2024-12-03T02:58:34.925Z"
  },
  {
    "content": "HelloV0.5",
    "date": "2024-12-03T03:05:30.862Z"
  },
  {
    "content": "Hello world",
    "date": "2024-12-03T03:11:00.184Z"
  },
  {
    "content": "hello again",
    "date": "2024-12-03T03:47:57.936Z"
  },
  {
    "content": "hello again",
    "date": "2024-12-03T03:48:13.254Z"
  },
  {
    "content": "whaat",
    "date": "2024-12-03T04:47:08.587Z"
  },
  {
    "content": "whaat",
    "date": "2024-12-03T04:47:48.393Z"
  },
  {
    "content": "whaat",
    "date": "2024-12-03T04:54:02.572Z"
  },
  {
    "content": "whaat",
    "date": "2024-12-03T05:11:35.919Z"
  },
  {
    "content": "Hello",
    "date": "2024-12-03T05:45:56.189Z"
  },
  {
    "content": "Hello",
    "date": "2024-12-03T05:45:56.521Z"
  },
  {
    "content": "thenewnote",
    "date": "2024-12-03T05:59:28.064Z"
  },
  {
    "content": "awholenewnote",
    "date": "2024-12-03T06:10:03.520Z"
  },
  {
    "content": "",
    "date": "2024-12-03T06:31:45.555Z"
  },
  {
    "content": "moo deng",
    "date": "2024-12-03T06:52:43.824Z"
  },
  {
    "content": "Sambamba",
    "date": "2024-12-03T06:52:49.258Z"
  },
  {
    "content": "Ok",
    "date": "2024-12-03T06:52:52.752Z"
  },
  {
    "content": "Yes",
    "date": "2024-12-03T06:53:01.716Z"
  },
  {
    "content": "Not OK",
    "date": "2024-12-03T06:53:11.082Z"
  },
  {
    "content": "GO BANANA",
    "date": "2024-12-03T06:56:03.703Z"
  },
  {
    "content": "look at network",
    "date": "2024-12-03T06:59:55.882Z"
  },
  {
    "content": "Testsave",
    "date": "2024-12-03T07:06:44.750Z"
  },
  {
    "content": "",
    "date": "2024-12-03T07:18:47.616Z"
  },
  {
    "content": "nikka 69",
    "date": "2024-12-03T07:19:22.026Z"
  },
  {
    "content": "yihaaoo!",
    "date": "2024-12-03T07:20:01.595Z"
  },
  {
    "content": "zimbo",
    "date": "2024-12-03T07:31:16.180Z"
  },
  {
    "content": "y",
    "date": "2024-12-03T08:10:20.365Z"
  },
  {
    "content": "",
    "date": "2024-12-03T08:16:08.103Z"
  },
  {
    "content": "dadad",
    "date": "2024-12-03T08:16:15.373Z"
  },
  {
    "content": "o",
    "date": "2024-12-03T08:20:36.409Z"
  },
  {
    "content": "lets go",
    "date": "2024-12-03T08:20:50.633Z"
  },
  {
    "content": "wat",
    "date": "2024-12-03T08:21:13.040Z"
  },
  {
    "content": "rrra",
    "date": "2024-12-03T08:25:39.102Z"
  },
  {
    "content": "ye",
    "date": "2024-12-03T08:25:43.518Z"
  },
  {
    "content": "testing",
    "date": "2024-12-03T08:41:45.393Z"
  },
  {
    "content": "what is it",
    "date": "2024-12-03T08:56:14.763Z"
  },
  {
    "content": "<h1>test</h1>",
    "date": "2024-12-03T09:20:53.982Z"
  },
  {
    "content": "",
    "date": "2024-12-03T09:22:23.138Z"
  },
  {
    "content": "dadad",
    "date": "2024-12-03T09:35:04.914Z"
  },
  {
    "content": "new note",
    "date": "2024-12-03T10:24:58.942Z"
  },
  {
    "content": "is this working",
    "date": "2024-12-03T10:44:36.957Z"
  },
  {
    "content": "from visual",
    "date": "2024-12-03T11:08:30.030Z"
  }
]
    deactivate server

