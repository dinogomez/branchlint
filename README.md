# Branchlint

A simple script to convert branch names into a desired format.

## Features
![image](https://github.com/dinogomez/branchlint/assets/41871666/c896c4b6-8f98-4c03-bfe1-00f7dcbc1c8a)

- Converts branch names like `64-bug-typed-errors-for-dynamic-typed-routing` into `bug/typed_errors_for_dynamic_typed_routing`.

## Installation

### Prerequisites

- A Unix-like operating system (Linux, macOS)
- Bash shell

### Steps

1. **Clone the repository:**

   ```bash
   git clone https://github.com/dinogomez/branchlint.git
   ```

2. **Navigate to the repository:**

   ```bash
   cd branchlint
   ```

3. **Make the script executable:**

   ```bash
   chmod +x branchlint
   ```

4. **Move the script to `/usr/local/bin` for global access:**

   ```bash
   sudo mv branchlint /usr/local/bin/
   ```

   You might need to enter your admin password.

5. **Ensure `/usr/local/bin` is in your `PATH`:**

   ```bash
   echo $PATH
   ```

   If `/usr/local/bin` is not listed in the output, add it to your shell configuration file (e.g., `.bash_profile`, `.zshrc`):

   ```bash
   export PATH="/usr/local/bin:$PATH"
   ```

   Then, reload your shell configuration:

   ```bash
   source ~/.bash_profile  # for Bash users
   source ~/.zshrc         # for Zsh users
   ```

#### Option 2: Set Up as an Alias

1. **Clone the repository:**

   ```bash
   git clone https://github.com/dinogomez/branchlint.git
   ```

2. **Navigate to the repository:**

   ```bash
   cd branchlint
   ```

3. **Make the script executable:**

   ```bash
   chmod +x branchlint
   ```

4. **Add an alias to your shell configuration file (e.g., `.bash_profile`, `.zshrc`):**

   ```bash
   alias branchlint="$(pwd)/branchlint"
   ```

5. **Reload your shell configuration:**

   ```bash
   source ~/.bash_profile  # for Bash users
   source ~/.zshrc         # for Zsh users
   ```

## Usage

Once the script is installed and in your `PATH`, you can use it from anywhere in your terminal.

```bash
branchlint <branch-name>
```
