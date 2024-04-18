## tmux
 **What is tmux?** Tmux stands for "terminal multiplexer." It's a command-line tool that allows you to split your terminal window into multiple panes or windows, enabling you to run multiple terminal sessions within one window. It's especially useful for managing multiple tasks or sessions on a remote server or when working with multiple command-line interfaces.

 **Basic tmux Commands:**
 
> 1. **Starting tmux:** Simply type `tmux` into your terminal and press Enter. This will start a new tmux session.
> 2. **Creating Windows:** Inside tmux, you can create multiple windows. Press `Ctrl + B`, then `c` to create a new window.
> 3. **Navigating Windows:** To navigate between windows, press `Ctrl + B`, then the window number (e.g., `0`, `1`, `2`, etc.).
> 4. **Splitting Panes:** You can split the current window into multiple panes. Press `Ctrl + B`, then `%` to split vertically or `"` to split horizontally.
> 5. **Moving between Panes:** To move between panes, press `Ctrl + B`, then an arrow key in the direction you want to move.
> 6. **Closing Panes:** To close a pane, you can simply exit the shell running inside it (`Ctrl + D`), or you can close it without exiting by pressing `Ctrl + B`, then `x`.
> 7. **Detaching from tmux:** If you want to leave tmux running in the background but detach from it, press `Ctrl + B`, then `d`. This will return you to your regular terminal session.
> 8. **Reattaching to tmux:** To reattach to a tmux session that you've detached from or that was running in the background, simply type `tmux attach` into your terminal and press Enter.
> 
> These are just a few basic commands to get you started with tmux. It's a powerful tool with many more features, so feel free to explore its documentation or online guides for more advanced usage.

To close a tmux session with ID 2, you need to first ensure that you're not currently attached to it. If you're not attached to the session, you can simply kill it using the tmux ```kill-session -t <session_id>``` command. Here's how to do it:

First, detach from any tmux session you might be attached to by pressing``` Ctrl + B, then d```.

Once you're back in your regular terminal, type the following command to kill the tmux session with ID 2:.

Copy code
```tmux kill-session -t 2```

**This command will terminate the tmux session with ID 2**.
