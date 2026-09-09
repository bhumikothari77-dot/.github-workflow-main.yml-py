name: Hello Workflow

on: [push]

jobs:
  greet:
    runs-on: ubuntu-latest
    steps:
      - name: Check out code
        uses: actions/checkout@v4

      - name: Print greeting
        run: echo "Hello from GitHub Actions!"

      - name: Print current date and time
        run: date

      - name: Print trigger branch name
        run: echo "Branch that triggered the run is ${{ github.ref_name }}"

      - name: List files in the repository
        run: ls -la

      - name: Print runner's operating system
        run: uname -a
