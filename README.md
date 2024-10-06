## Cat Volleyball
- A simple 2D volleyball game build in Rust using the Bevy game engine, inspired by the classic "Pikachu Volleyball"

### Features
*   2D graphics with sprite animation
*   Two-player gameplay
*   Simple physics simulation (ball movement, bouncing)
*   Scorekeeping
*   Sound effects
## Local System Setup
### Installation and setup
1.  **Install Rust**: https://www.rust-lang.org/tools/install

2.  **Install System Dependencies**: Bevy requires several system-level libraries for graphics, audio, etc. 
    #### For Ubuntu 20.04:
    ```bash
    sudo apt install g++ pkg-config libx11-dev libasound2-dev libudev-dev
    ```

    #### For Debian-based systems:
    ```bash
    sudo apt install g++ pkg-config libx11-dev libasound2-dev libudev-dev
    ```

    #### For Red Hat-based systems:
    ```bash
    sudo yum install gcc-c++ pkgconfig libX11-devel alsa-lib-devel libudev-devel
    ```

    #### For Arch-based systems:
    ```bash
    sudo pacman -S gcc pkgconf libx11 alsa-lib libudev
    ```
3. **Clone the repository**:
    ```bash
    git clone https://github.com/kishore-1404/Building-A-Game.git
    cd Building-A-Game
    ```
4. **Run the game**:
    ```bash
    cargo run --release
    ```
5. **Design**:

*   Two players control cat avatars on opposite sides of the screen.
*   Players can move left and right and jump to hit the ball.
*   The ball follows a parabolic trajectory affected by gravity.
*   The first player to reach a certain score wins the game.

## GitHub Repository
- This is guided tutorial to build a simple 2D volleyball game in Rust using the Bevy game engine.
- Simply clone this template repository and follow the instructions in the README.md file to build the game.

### Instructions
1. open `cargo.toml` file and add the following dependencies:
```toml
[dependencies]
bevy = "0.5"
```
2. open `src/main.rs` file and add the following code:
```rust
use bevy::prelude::*;

fn main() {
    App::new()
        .add_plugins(DefaultPlugins)
        .run();
}
```
After adding the above changes , comit and push the changes to the repository. GitHub actions will verify progress and update the `README.md` .