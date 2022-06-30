# Getting-started-with-tmux

Tmux is a terminal multiplexer. Tmux allows a number of terminals  each running a separate program, to be created and used inside a session. It allows switching between multiple programs in one terminal, detach them and reattach them to a different terminal.

As tmux sessions are presistent, programs running in Tmux will continue to run even if you get disconnected.


### Installation of tmux
#### On Ubuntu and Debian
```$ sudo apt install tmux```

#### On Fedora and CentOS
```$ sudo yum install tmux```

#### On MacOS
```$ brew install tmux```

### Session on tmux
To start a sesson on tmux use command <br>
```$ tmux```

Once the session is started, status line at the bottom of the screen shows information about the current session.

#### Named sessions
Named sessions can be created using command <br>
```$tmux new -s new-session-name```

`ctrl` + `b` **is the prefix of tmux. All command begin with prefix by default**

### Commands for pane
| Command | Description |
|---------|--------------|
| `prefix`+ `?`| Shows list of all availabe commands|
| `prefix`+ `c`| Creates a new window|
| `prefix`+ `%`| Splits window vertically|
| `prefix`+ `"`| Splits window horizontally|
| `prefix`+ `→`| Moves to right pane|
| `prefix`+ `←`| Moves to left pane|
| `prefix`+ `↑`| Moves to upper pane|
| `prefix`+ `↓`| Moves to lower pane|


### More about sessions
Once we type command `$tmux` the session starts. We can then see green bar at the bottom. This bar indicates the active session, and that we are using Tmux. 


To find active tmux sessions use command<br>
```$tmux ls```

If you want to start a attached session use command<br>
```$tmux attach -t name-of-the-session```

To kill a tmux session use command<br>
```$tmux kill-session -t name-of-the-session```

Finally to exit out of the session, simply type<br>
```$exit```

### Conclusion
Tmux is an important tool that helps to use single terminal  by splitting windows and navigating through sessions.
To explore more about tmux you can visit [official documentation](https://tmuxguide.readthedocs.io/en/latest/tmux/tmux.html).
