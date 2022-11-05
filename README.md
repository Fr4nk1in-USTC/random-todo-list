# random-todo-list

> This is an RANDOM repository. Maybe no progress would be made.

> I have no idea what it is. I know little about real-world software development. Feel free to create new [issues](https://github.com/Fr4nk1in-USTC/random-todo-list/issues/new) or pull requests if you have any suggestion, idea or guidance.

## Inspiration

I'm using [Obsidian](https://obsidian.md/) for note taking and task/todo management. However, since I don't take notes very often, I decide to use a separate application to manage my task/todo/timeline. I haven't found a finished application to meet all my expectations, so I would try to make one myself.

## Expectation

### Functions

> All the tasks should be stored in a readable file.

As a todo-list application, it can

- Create new tasks
- Delete existing tasks
- Click to finish
- Set deadline / priority of tasks
- Attach certain application / command to a task
  - For example, `code ~/project/random-project` for a code task.
- Assign categories to tasks
- [Want more or have any idea?](https://github.com/Fr4nk1in-USTC/random-todo-list/issues/new)

### UI

> GUI? TUI? I don't know.

```plaintext
╭───┬──────────────────────────────────────┬─╮
│ □ │ TODO List                            │+│
├───┼──────────────────────────────────────┴─┤
│ □ │╭──────────────────────────────────────╮│
│ □ ││ □ Task1                           ▹ …││
│ □ │╰──────────────────────────────────────╯│
│ □ │╭──────────────────────────────────────╮│
│ □ ││ □ Task2                             …││
│   │╰──────────────────────────────────────╯│
│   │╭──────────────────────────────────────╮│
│   ││─────────────────────────────────────…││
│   │╰──────────────────────────────────────╯│
│   │                                        │
│   │                                        │
│   │                                        │
│   │                                        │
│   │                                        │
│   │                                        │
│   │                                        │
│   │                                        │
│   │                                        │
│   │                                        │
╰───┴────────────────────────────────────────╯
```

- The classic plain layout (shown as above)
- The catagory layout
  ```plaintext
  ╭───┬──────────────────────────────┬─╮
  │ □ │ Catagories                   │+│
  ├───┼──────────────────────────────┴─┤
  │ □ │╭──────────────╮╭──────────────╮│
  │ □ ││ CATA1    + … ││ CATA2    + … ││
  │ □ ││╭────────────╮││╭────────────╮││
  │ □ │││ □ Task1 ▹ …││││ □ Task1 ▹ …│││
  │ □ ││╰────────────╯││╰────────────╯││
  │   ││╭────────────╮││╭────────────╮││
  │   │││ □ Task2   …││││───────────…│││
  │   ││╰────────────╯││╰────────────╯││
  │   ││╭────────────╮│╰──────────────╯│
  │   │││───────────…││╭──────────────╮│
  │   ││╰────────────╯││ CATA3    + … ││
  │   │╰──────────────╯│╭────────────╮││
  │   │                ││ □ Task1 ▹ …│││
  │   │                │╰────────────╯││
  │   │                │╭────────────╮││
  │   │                ││───────────…│││
  │   │                │╰────────────╯││
  │   │                ╰──────────────╯│
  │   │                                │
  │   │                                │
  │   │                                │
  ╰───┴────────────────────────────────╯
  ```
  Click to expand:
  ```plaintext
  ╭───┬──────────────────────────────┬─╮
  │ □ │ Catagories                   │+│
  ├───┼──────────────────────────────┴─┤
  │ □ │╭──────────────╮╭──────────────╮│
  │ □ ││ CATA1    + … ││ CATA2    + … ││
  │ □ ││╭────────────╮││╭────────────╮││
  │ □ │││ □ Task1 ▹ …││││ □ Task1 ▹ …│││
  │ □ ││╰────────────╯││╰────────────╯││
  │   ││╭────────────╮││╭────────────╮││
  │   │││ □ Task2   …││││───────────…│││
  │   ││╰────────────╯││╰────────────╯││
  │   ││╭────────────╮│╰──────────────╯│
  │   │││───────────…││╭──────────────╮│
  │   ││╰────────────╯││ CATA3    + … ││
  │   │╰──────────────╯│╭────────────╮││
  │   │                ││ □ Task1 ▹ …│││
  │   ├────────────────────────────────┤
  │   │ CATA1                      + … │
  │   │╭──────────────────────────────╮│
  │   ││ □ Task1                   ▹ …││
  │   │╰──────────────────────────────╯│
  │   │╭──────────────────────────────╮│
  │   ││ □ Task2                     …││
  │   │╰──────────────────────────────╯│
  ╰───┴────────────────────────────────╯
  ```
- The [Eisenhower Matrix](https://en.wikipedia.org/wiki/Time_management#The_Eisenhower_Method) layout
  > Dots or small rectangles?
  ```
  ╭───┬─────────────────────────────────────────╮
  │ □ │ Urgency/Importance Matrix               │
  ├───┼─────────────────────────────────────────┤
  │ □ │        Urgent                           │
  │ □ │I     .             │               .    │
  │ □ │m   .               │           .        │
  │ □ │p                   │     .              │
  │ □ │o      .            │         .          │
  │   │r           .       │                    │
  │   │t                 . │                    │
  │   │ ───────────────────┼─────────────────── │
  │   │                    │                    │
  │   │    .     . .       │    .          .    │
  │   │                    │        .           │
  │   │    .               │             .      │
  │   │       .            │  .                 │
  │   │                    │                    │
  │   │                    │                    │
  │   │                                         │
  │   ├─────────────────────────────────────────┤
  │   │ □ Task1                              ▹ …│
  ╰───┴─────────────────────────────────────────╯
  ```
- Timeline/Calendar (click to change the main frame to Today/Week/Month)
  ```
  ╭───┬─────────────────────────────────────────╮
  │ □ │ Timeline                                │
  ├───┼─────────────────────────────┬─┬─────────┤
  │ □ │ Today                       │+│ Month   │
  │ □ ├─────────────────────────────┴─┤   12345 │
  │ □ │ 10:15 ─────────────────────── │ 6789012 │
  │ □ │ ╭────────────────────────────╮│ 3456789 │
  │ □ │ │──────────────────────── ▹─…││ 0123456 │
  │   │ ╰────────────────────────────╯│ 78901   │
  │   │ 14:00 ─────────────────────── ├─────────┤
  │   │ ╭────────────────────────────╮│ Week    │
  │   │ │ □ Task                  ▹ …││ │       │
  │   │ ╰────────────────────────────╯│ ├────── │
  │   │ 14:30 ─────────────────────── │▹├────── │
  │   │ ╭────────────────────────────╮│ │       │
  │   │ │ □ Task                  ▹ …││ │       │
  │   │ ╰────────────────────────────╯│ ├────── │
  │   ├───────────────────────────────┤ ├────── │
  │   │ Today                   14:12 │ │       │
  │   │                  ▿            │ ├────── │
  │   │ ────┬─────┬────┬──┬────┬───── │ │       │
  │   │     │     │    │  │    │      │ │       │
  │   │     │     │    │  │    │      │ │       │
  │   │     │     │    │  │    │      │ │       │
  │   │     │     │    │  │    │      │ │       │
  │   │     │     │    │  │    │      │ ├────── │
  ╰───┴───────────────────────────────┴─────────╯
  ```

## Project Framework

> WTF is a framwork?

- Cross platform: Tauri? Electron? Qt? .Net?
- Or specific platform: WinAPI? GTK?

## TODO

- [ ] Determain everything.
- [ ] Prepare everything.
- [ ] Learn how to build a real project.
- [ ] Code!
