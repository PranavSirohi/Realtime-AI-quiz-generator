<img src="assets/logo.svg" width="100%" height="80px">

# REALTIME AI QUIZ GENERATOR


> Real time quiz application

## 📜 Table of Contents

- [🌟 Introduction](#-introduction)
- [✨ Features](#-features)
- [⚙️ Build Instructions](#-build-instructions)

## 🌟 Introduction 

An **interactive, real-time multiplayer quiz platform** powered by **AI**.  
Built to create fun, engaging, and intelligent quizzes for classrooms, events, or online learning.  


## ✨ Features

- **Small and Performant**: Binary sizes for Windows and Linux are optimized, ensuring efficiency without sacrificing performance.
- **Name Filtering**: Maintain a positive environment by customizing the level of filtering for player usernames on a per-quiz basis.
- **Image Fitting**: Adapt quiz images for various devices with options like Cover, Contain, Fit Width, and Fit Height.
- **Customization Options**:
  - Adjust time limits for answering questions.
  - Set min, max, and bonus scores for each question.
  - Support for different question types: Single, Multiple, True/False, and Typer.
- **Easy Shuffling**: Quickly rearrange the order of questions and answers for variety.
- **Readiness and Preloading**: Ensure fairness by waiting for all players to preload images before starting question timers.
- **Fully Portable**: No files are persisted, making Quizler completely portable as a single executable. Quizzes can be exported/imported as self-contained .quizler files.
- **Containerized**: Run Quizler as a standalone executable or within a Docker container using the `jacobtread/quizler` container image. Example `docker-compose.yml` provided.
- **Short and Shareable Codes**: Quiz codes consist of short 5-character tokens (e.g., AZ2ES), making sharing easy.
- **Cross-Platform**: Server runs on both Windows and Linux, accessible from any device with a web browser.


## ⚙️ Build Instructions

Building Quizler requires NodeJS (>=16) for the frontend and Cargo/Rust (>=1.75.0) for the backend:

1. **Frontend**:
    ```shell
    # Move to the frontend directory
    cd frontend
    # Install dependencies 
    npm install
    # Run the dist commands
    npm run dist
    # Move out of the frontend directory
    cd ..
    ```

2. **Backend**:
    ```shell
    # Move to the backend directory
    cd backend
    # Build the release binary
    cargo build --release
    ```

For Docker-based builds, refer to the provided `Build.Dockerfile` in the repository, there is also
a docker image for pre-built binaries at `Dockerfile`.


OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
