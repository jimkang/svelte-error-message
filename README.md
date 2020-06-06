# svelte-error-message

Super basic error message displaying component that I created mostly to avoid having to copy everywhere.

## Installation

    npm install svelte-error-message

## Usage

    <script>
    import ErrorMessage from 'svelte-error-message';

    let error;

    if (somethingIsWrong()) {
      // When this is set, the error message will display on the page.
      // Otherwise, nothing will display.
      error = new Error('Something is wrong');
    }
    </script>

    <div>
      <ErrorMessage error={error} />
    </div>

## Properties

- `error`: [An error](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Error) or something that has the same properties.

## License

The MIT License (MIT)

Copyright (c) 2020 Jim Kang

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the 'Software'), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
