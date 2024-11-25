# PuTTY

Forward Movement

    Press ESC followed by f to move forward one word3
    Alternatively, use Alt + Right Arrow1

Backward Movement

    Press ESC followed by b to move backward one word3
    Alternatively, use Alt + Left Arrow1

If the Alt + Arrow key combinations aren't working properly, you can configure them using the bind command:

```sh
bash
bind '"\e\e[D":backward-word'
bind '"\e\e[C":forward-word'
```[1]

These bindings should be added to your `.bashrc` file to make them
permanent. If you need to identify the exact key codes your terminal is
generating, you can use the `cat > /dev/null` command and press the key
combination to see the output[1].
```

```sh
echo 'bind "\"\\e\\e[D\":backward-word"' >> ~/.bashrc
echo 'bind "\"\\e\\e[C\":forward-word"' >> ~/.bashrc

source ~/.bashrc
```
