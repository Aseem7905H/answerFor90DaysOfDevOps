To set your username and email address for Git, you can use the following commands:

### Global Configuration (for all repositories):

```bash
git config --global user.name "Your Name"
git config --global user.email "youremail@example.com"
```

### Local Configuration (for the current repository only):

Navigate to the directory of your Git repository and run:

```bash
git config user.name "Your Name"
git config user.email "youremail@example.com"
```

### To verify the configuration:
You can check if the configuration was successful using the command:

```bash
git config --list
```

This will display your Git configuration settings, including your username and email address.
