Certain scenarios will require multiple terminal tabs to be running. These can be opened dynamically using the Markdown Extensions, but they can also be opened when the scenario starts.

## Terminal Tab

The index.json supports the following syntax that allows you to define an additional terminal tab.

"environment": {
  "terminals": [{"name": "Terminal 2", "target": "host01"}]
}
## Automatically Run Commands

These tabs can automatically run certain commands to help the user understand what is happening. The command below will open a new Terminal tab and automatically run docker stats command.

"environment": {
  "terminals": [{"name": "Docker Stats", "command": "docker stats", "target": "host01"}]
}
The can be used for tasks such as watching a event stream, or viewing all the processes running on a system.

Within the Markdown content for Katacoda you can embed any HTML element, this means you would have the ability to embed YouTube videos, such as the example below.

<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/KeJJ34BvA7Q" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
The HTML included is:

<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/KeJJ34BvA7Q" frameborder="0" allow="accelerometer; autoplay; encrypted-med
