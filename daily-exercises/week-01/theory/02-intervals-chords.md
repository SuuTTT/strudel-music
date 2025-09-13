# Day 2: Intervals and Chord Building

## Learning Objective
Understand intervals (distances between notes) and how they form chords.

## Music Theory

### Intervals
An interval is the distance between two notes:
- **Unison**: Same note (0 semitones)
- **Minor 2nd**: 1 semitone (C to C#)
- **Major 2nd**: 2 semitones (C to D)
- **Minor 3rd**: 3 semitones (C to Eb)
- **Major 3rd**: 4 semitones (C to E)
- **Perfect 4th**: 5 semitones (C to F)
- **Perfect 5th**: 7 semitones (C to G)
- **Octave**: 12 semitones (C to C)

### Basic Triads
- **Major Chord**: Root + Major 3rd + Perfect 5th (C + E + G)
- **Minor Chord**: Root + Minor 3rd + Perfect 5th (C + Eb + G)

## Strudel Harmony

### Playing Intervals
```javascript
// Perfect 5th (C and G together)
stack(note("c"), note("g"))

// Major 3rd (C and E together)
stack(note("c"), note("e"))

// Octave (C and C)
stack(note("c3"), note("c4"))
```

### Building Chords
```javascript
// C Major chord
stack(note("c"), note("e"), note("g"))

// A Minor chord
stack(note("a"), note("c5"), note("e5"))

// Chord progressions
sequence(
  stack(note("c"), note("e"), note("g")),    // C Major
  stack(note("f"), note("a"), note("c5")),   // F Major
  stack(note("g"), note("b"), note("d5")),   // G Major
  stack(note("c"), note("e"), note("g"))     // C Major
)
```

## Exercises

### Exercise 1: Interval Recognition
```javascript
// Listen to these intervals - can you hear the difference?
stack(note("c"), note("d")).slow(2)  // Major 2nd
stack(note("c"), note("e")).slow(2)  // Major 3rd
stack(note("c"), note("f")).slow(2)  // Perfect 4th
stack(note("c"), note("g")).slow(2)  // Perfect 5th
```

### Exercise 2: Major vs Minor
```javascript
// C Major chord
stack(note("c"), note("e"), note("g")).slow(2)

// C Minor chord (notice the Eb instead of E)
stack(note("c"), note("eb"), note("g")).slow(2)
```

### Exercise 3: Simple Chord Progression
```javascript
// I-V-vi-IV progression (very common!)
sequence(
  stack(note("c"), note("e"), note("g")),    // C Major (I)
  stack(note("g"), note("b"), note("d5")),   // G Major (V)
  stack(note("a"), note("c5"), note("e5")),  // A minor (vi)
  stack(note("f"), note("a"), note("c5"))    // F Major (IV)
).slow(2)
```

## Practice Tasks
1. Build major chords starting on D, E, F, G
2. Build minor chords starting on A, B, C, D
3. Listen to interval differences
4. Create a 4-chord progression