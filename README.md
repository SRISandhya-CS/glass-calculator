# Glass Calculator

A modern calculator built with HTML, CSS, and JavaScript — featuring a glassmorphism interface, smart expression parsing, and a full calculation history tape.

## Features

### Smart Expression Parsing
Type or click full algebraic expressions like `5 * (3 + 2)` instead of pressing one operation at a time. The calculator correctly handles:
- Operator precedence (multiplication/division before addition/subtraction)
- Parentheses for grouping
- Exponents (`^`)
- Percentages (`%`)
- Negative numbers

Expressions are evaluated using a custom-built parser (tokenizer + shunting-yard algorithm), not JavaScript's `eval()` — so the math is handled safely rather than executing raw code.

### Live Ghost Preview
As you type, a faint preview of the result appears below the input before you even press `=`, so you can sanity-check your expression as you build it.

### Editable History Tape
Every calculation you run is saved in a sidebar tape showing the original expression and its result. Click any past result to drop it straight back into the input and keep building on it.

### Full Keyboard Support
Mouse-free from start to finish:
| Key | Action |
|---|---|
| `0-9`, `+ - * / ^ % ( )` | Insert into expression |
| `Enter` | Evaluate (`=`) |
| `Backspace` | Delete last character |
| `Escape` | Clear input |

### Dark / Light Mode
A toggle switch swaps the entire color palette — including the background gradient blobs that the glass panels blur — between a dark indigo/pink theme and a soft light theme.

## How to Use

Just open `glass-calculator.html` in any modern browser. No installation, no build step, no dependencies beyond a Google Fonts link for typography.

## Tech Stack

- **HTML** — structure
- **CSS** — glassmorphism styling (backdrop blur, gradients, responsive layout), dark/light theming via CSS variables
- **JavaScript** — expression parsing/evaluation, input handling, history tape logic, theme switching

## File Structure

This is a single self-contained file — all HTML, CSS, and JavaScript live in `glass-calculator.html`. No separate files needed.
