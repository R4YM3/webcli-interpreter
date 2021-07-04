# web-cli-interpreter

A package which will interpreted a given string as a command and will run it on given programs.

_note: this project is still under heavy development_

```
import { init, programs as defaultPrograms } from "web-cli-interpreter";

const whoami = defaultPrograms.whoami({
    info: `<p>
      Spare time project of Raymond Schweers.<br/>
      To explore, learn and seek new technologies and by doing so creating a handy<br/>
      command line interface build with: TypeScript, React, and Sass
    </p>`,
});

const interpret = init({
    programs: [whoami],
});

interpret(shell.command.value);

```

## Interpertation of given string
A given command should be in the following scheme:
`program method1 --arg1 arg1value -arg2 arg2value method2 --arg1 value1`

tbd..

## Creating your own programs
`import { Program } from "web-cli-interpreter";`

Create a new instance and add the program in programs array in init() function.

tbd..