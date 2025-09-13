# Day 1: Basic Patterns and Sequencing

## Learning Objective
Master the fundamental Strudel pattern syntax and sequencing methods.

## Core Concepts

### Pattern Creation
Strudel works with patterns - sequences of musical events that can loop and transform.

### Basic Syntax Elements
- **Strings**: `"c d e f"` - Space-separated sequences
- **Arrays**: `["c", "d", "e", "f"]` - Comma-separated elements  
- **Functions**: `.slow()`, `.fast()`, `.rev()` - Transform patterns

## Essential Strudel Functions

### Pattern Creation
```javascript
// Basic pattern
note("c d e f")

// Equivalent array notation
note(["c", "d", "e", "f"])

// Rest/silence
note("c ~ e ~")  // ~ represents silence
```

### Timing Controls
```javascript
// Slow down (longer notes)
note("c d e f").slow(2)    // 2x slower
note("c d e f").slow(4)    // 4x slower

// Speed up (shorter notes)
note("c d e f").fast(2)    // 2x faster
note("c d e f").fast(4)    // 4x faster
```

### Pattern Transformations
```javascript
// Reverse the pattern
note("c d e f").rev()

// Repeat each element
note("c d e f").echo(2)
```

## Today's Exercises

### Exercise 1: Basic Patterns
```javascript
// Try each of these patterns:
note("c d e f")
note("c e g c5")
note("c ~ e ~ g ~ c5 ~")
```

### Exercise 2: Timing Experiments
```javascript
// Compare these different speeds:
note("c d e f g a b c5").slow(4)   // Very slow
note("c d e f g a b c5").slow(2)   // Slow
note("c d e f g a b c5")           // Normal
note("c d e f g a b c5").fast(2)   // Fast
note("c d e f g a b c5").fast(4)   // Very fast
```

### Exercise 3: Pattern Transformations
```javascript
// Original pattern
note("c e g f a d g c5")

// Try these transformations:
note("c e g f a d g c5").rev()
note("c e g f a d g c5").echo(2)
note("c e g f a d g c5").slow(2).rev()
```

### Exercise 4: Combining Patterns
```javascript
// Stack patterns (play simultaneously)
stack(
  note("c e g c5"),
  note("c2 f2 g2 c3").slow(2)
)

// Sequence patterns (play one after another)
sequence(
  note("c d e f"),
  note("g a b c5")
)
```

## Practice Tasks

1. **Create** 3 different 4-note patterns
2. **Experiment** with different `.slow()` and `.fast()` values
3. **Try** combining `.rev()` with timing changes
4. **Build** a simple call-and-response pattern using `sequence()`

## Common Patterns to Master

```javascript
// Ascending pattern
note("c d e f g a b c5")

// Descending pattern  
note("c5 b a g f e d c")

// Skipping pattern
note("c e g c5 g e")

// Rhythmic pattern with rests
note("c ~ c ~ e ~ e ~")
```

## Notes Section
```
Pattern ideas I discovered:
- 
- 
- 

Interesting transformations:
- 
- 
```