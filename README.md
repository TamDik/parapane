# parapane
Parapane is a command for tmux users to run programs in parallel in their respective panes.

## Example

configuration format
```
[command]
exec="echo this is 1st pane"

[command]
exec="echo this is 2nd pane"

[command]
exec="echo this is 3rd pane";some comments

[sleep]
sec=2

[command]
exec="echo this is 4th pane"
```

use a config file
```sh
parapane path_to_config
```

use a pipeline
```sh
cat path_to_config | parapane
```

![parapage](https://user-images.githubusercontent.com/59227885/116732501-da6cb000-aa25-11eb-9bbb-ad52ba738ba2.gif)
