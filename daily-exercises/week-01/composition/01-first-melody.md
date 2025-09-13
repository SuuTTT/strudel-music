# Day 1: Creating Your First Melody

## Learning Objective
Apply music theory and syntax knowledge to create a simple, expressive melody.

## Composition Principles

### Melody Basics
- **Direction**: Melodies move up, down, or stay the same
- **Steps vs Leaps**: Small intervals (steps) vs large intervals (leaps)
- **Shape**: The overall contour of the melody
- **Repetition**: Repeating elements create familiarity

### Simple Song Forms
- **ABAB**: Verse-Chorus structure
- **AABA**: Common pop song form
- **Call and Response**: Question-answer musical phrases

## Composition Techniques in Strudel

### Creating Melodic Motion
```javascript
// Stepwise motion (smooth)
note("c d e f g a b c5")

// Leaps (more dramatic)
note("c g e c5 a f d g")

// Mixed motion (most interesting)
note("c d f e g a f g")
```

### Building Musical Phrases
```javascript
// 4-beat phrase
note("c e g e").slow(2)

// 8-beat phrase
note("c d e f g f e d").slow(2)

// Question and answer
sequence(
  note("c d e f"),     // Question (rises)
  note("g f e c")      // Answer (falls back home)
)
```

## Today's Composition Exercises

### Exercise 1: Simple 4-Note Patterns
Create melodies using only 4 different notes from C major:
```javascript
// Example: Using C, E, G, A
note("c e g a g e c e")

// Your turn: Try D, F, A, B
note("d f a b a f d f")

// Create your own 4-note set:
note("_____ _____ _____ _____")
```

### Exercise 2: Question and Answer
```javascript
// Question phrase (ends on a note that wants to resolve)
const question = note("c d e f")

// Answer phrase (resolves back to home)
const answer = note("g f e c")

// Play them together
sequence(question, answer)
```

### Exercise 3: ABA Form
```javascript
// A section
const sectionA = note("c e g e f d e c")

// B section (contrasting)
const sectionB = note("g a b c5 b a g f")

// Complete ABA form
sequence(sectionA, sectionB, sectionA)
```

### Exercise 4: Adding Rhythm
```javascript
// Same melody with different rhythms
note("c e g e").slow(2)           // Slow and flowing
note("c ~ e ~ g ~ e ~").slow(1)   // With rests
note("c c e e g g e e").fast(1)   // Repeated notes
```

## Creative Challenges

### Challenge 1: Emotional Direction
Create melodies that express different emotions:
```javascript
// Happy melody (ascending, bouncy)
note("c e g c5 g e c g").fast(1.5)

// Sad melody (descending, slower)
note("c5 b a g f e d c").slow(2)

// Your mysterious melody:
note("_____________")
```

### Challenge 2: Musical Conversation
```javascript
// High voice
const voice1 = note("c5 d5 e5 f5")

// Low voice responding
const voice2 = note("c3 f3 g3 c3")

// Play conversation
stack(
  voice1.slow(2),
  voice2.slow(2).late(0.5)  // Start slightly later
)
```

### Challenge 3: Developing a Motif
Start with a simple idea and develop it:
```javascript
// Original motif
const motif = note("c e g")

// Variations
motif.rev()                    // Backwards
motif.echo(2)                  // Repeated
motif.slow(2)                  // Stretched
note("c e g c5 e5 g5")        // Extended higher
```

## Composition Checklist

When creating a melody, ask yourself:
- [ ] Does it have a clear starting and ending point?
- [ ] Are there both steps and leaps for interest?
- [ ] Does it have a memorable shape or contour?
- [ ] Can I sing or hum it easily?
- [ ] Does it resolve satisfyingly?

## Today's Composition Project

**Create a 16-beat melody that tells a musical story:**

```javascript
// Your composition here:
// Use sequence() or stack() to create sections
// Include both stepwise motion and leaps
// End on a satisfying resolution note

const myMelody = sequence(
  note("______"),  // Opening phrase
  note("______"),  // Development
  note("______"),  // Climax
  note("______")   // Resolution
)
```

## Reflection Notes
```
What story did my melody tell?
- 

What techniques worked well?
- 

What would I change next time?
- 

Ideas for tomorrow:
- 
```