name: CI Pipeline

on: push

jobs:
  greet:
    runs-on: ubuntu-latest
    steps:
      - name: Greet
        run: echo "Hello Bhumi!"

  build:
    runs-on: ubuntu-latest
    needs: greet
    steps:
      - name: Build
        run: echo "Building the application..."

      - name: Test
        run: echo "Running tests..."
