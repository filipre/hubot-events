# hubot-events

Hubot script to call and register hubot events.

See [`src/events.coffee`](src/events.coffee) for full documentation.

## Commands

```
hubot events add name=<name> event=<event> interval=<interval>- Add an event
hubot events remove name=<name>- Remove an event
hubot events list - Show all registered events
hubot events trigger name=<name> - Trigger a specific event by name
hubot events trigger event=<event> - Trigger a specific event by name
```

Notice that
- `name` musn't contain spaces
- `interval` has to be a cron expression like `0 0 * * * *`

## Installation

In hubot project repo, run:

`npm install hubot-events --save`

Then add **hubot-events** to your `external-scripts.json`:

```json
[
  "hubot-events"
]
```
