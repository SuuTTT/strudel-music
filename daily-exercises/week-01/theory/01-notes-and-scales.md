# Day 1: Notes and Scales

## Learning Objective
Understand basic note names and how to represent them in Strudel code.

## Music Theory

### The Musical Alphabet
Music uses 7 letter names: A, B, C, D, E, F, G

### Chromatic Scale (All 12 Notes)
C, C#, D, D#, E, F, F#, G, G#, A, A#, B

### Major Scale Pattern
Whole-Whole-Half-Whole-Whole-Whole-Half (W-W-H-W-W-W-H)

## Strudel Syntax

### Basic Note Notation
```javascript
// Single notes
note("c")
note("d")
note("e")

// With octave numbers
note("c4")  // Middle C
note("c5")  // C one octave higher
note("c3")  // C one octave lower
```

### Playing Sequences
```javascript
// C major scale
note("c d e f g a b c5")

// Same scale with explicit octave
note("c4 d4 e4 f4 g4 a4 b4 c5")
```

## Today's Exercises

### Exercise 1: Play the C Major Scale
```javascript
// Copy this into Strudel and listen
note("c d e f g a b c5").slow(2)
```

### Exercise 2: Different Octaves
```javascript
// Try the same scale in different octaves
stack(
  note("c3 d3 e3 f3 g3 a3 b3 c4"),
  note("c4 d4 e4 f4 g4 a4 b4 c5"),
  note("c5 d5 e5 f5 g5 a5 b5 c6")
).slow(2)
```

### Exercise 3: Your First Melody
Create a simple melody using only notes from C major scale:
```javascript
// Example melody - modify this!
note("c e g e f d e c").slow(1)
```

## Practice Tasks

1. **Listen** to the C major scale - can you hear the pattern?
2. **Experiment** with different octaves
3. **Create** your own 8-note melody using C major scale notes
4. **Try** changing the tempo with `.slow()` and `.fast()`

## Next Steps
Tomorrow we'll learn about rhythm and timing patterns.

## Notes Section
(Write your observations and experiments here)

```
Today I learned:
- 
- 
- 

My melody creation:

```