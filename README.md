### This is a quick guide on how to set up your environment variables on macOS after installing Android Studio.

**Zsh Setup**
1. Create or open your `.zshrc` file:
```shell
touch ~/.zshrc; open ~/.zshrc
```
2. Insert the following lines into the opened `.zshrc` file:
```zsh
# Set the JAVA_HOME variable to the location of Android Studio's embedded JDK
export JAVA_HOME=/Applications/Android\ Studio.app/Contents/jbr/Contents/Home

# Add Android SDK platform-tools to the PATH
export PATH="$HOME/Library/Android/sdk/platform-tools:$PATH"
```
3. Optional: Verify the Android SDK Path (modify if necessary):
```zsh
# Make sure to update the path below if your Android SDK is located in a different directory
export PATH="$HOME/path/to/your/Android/sdk/platform-tools:$PATH"
```

4. Apply changes immediately by sourcing the `.zshrc` file:
```shell
source ~/.zshrc
```
