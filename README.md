# Strudel Music Learning Journey

A comprehensive resource for learning music theory, composition, and live coding with [Strudel](https://strudel.cc) - the web-based live coding environment for algorithmic music.

## 🎵 What is Strudel?

Strudel is a powerful JavaScript-based live coding language designed for making music in the browser. It allows you to:
- Create complex musical patterns with simple code
- Live code music performances
- Learn music theory through programming
- Experiment with algorithmic composition

## 📚 Learning Resources

### Daily Exercises
The `daily-exercises/` directory contains a structured 4-week learning program:

- **Week 1**: Foundations (notes, scales, basic patterns)
- **Week 2**: Harmony & Structure (chords, progressions, song form)  
- **Week 3**: Rhythm & Dynamics (complex rhythms, effects)
- **Week 4**: Advanced Techniques (modes, live coding, full compositions)

Each week includes:
- **Theory**: Music fundamentals explained clearly
- **Syntax**: Strudel programming techniques  
- **Composition**: Creative exercises and projects

### Quick Start
1. Visit [strudel.cc](https://strudel.cc) to access the Strudel environment
2. Start with `daily-exercises/week-01/theory/01-notes-and-scales.md`
3. Follow the exercises sequentially
4. Practice daily for 15-30 minutes

## 🎯 Learning Objectives

By completing this course, you will:
- ✅ Understand fundamental music theory concepts
- ✅ Master Strudel syntax and programming patterns
- ✅ Be able to convert musical ideas into Strudel code
- ✅ Create original compositions using live coding techniques
- ✅ Understand how code can express musical structure and emotion

## 🗂️ Repository Structure

```
strudel-music/
├── README.md              # This overview document
├── CHANGELOG.md           # Project updates and changes
└── daily-exercises/       # Structured learning program
    ├── README.md          # Exercise overview and instructions
    ├── week-01/           # Foundation week
    │   ├── theory/        # Music theory basics
    │   ├── syntax/        # Strudel programming
    │   └── composition/   # Creative exercises
    ├── week-02/           # Harmony & structure
    ├── week-03/           # Rhythm & dynamics
    └── week-04/           # Advanced techniques
```

## 🎼 From Music to Code

One of the main goals is learning to translate musical ideas into Strudel code. Here are some quick examples:

### Simple Melody
```javascript
// Musical idea: C major scale ascending
note("c d e f g a b c5")
```

### Chord Progression
```javascript
// Musical idea: I-V-vi-IV progression in C major
sequence(
  stack(note("c"), note("e"), note("g")),    // C major
  stack(note("g"), note("b"), note("d5")),   // G major  
  stack(note("a"), note("c5"), note("e5")),  // A minor
  stack(note("f"), note("a"), note("c5"))    // F major
)
```

### Rhythmic Pattern
```javascript
// Musical idea: Simple drum pattern
stack(
  sound("bd").struct("x~x~"),        // Kick on 1 and 3
  sound("hh").struct("~~~~~~~~"),     // Hi-hat on every 8th note
  sound("sd").struct("~x~x")         // Snare on 2 and 4
)
```

## 🚀 Getting Started

1. **Set up Strudel**: Go to [strudel.cc](https://strudel.cc)
2. **Start learning**: Begin with Week 1, Day 1 exercises
3. **Practice regularly**: Consistency is key for music learning
4. **Experiment freely**: Modify examples and create your own patterns
5. **Share your work**: Music is meant to be shared and enjoyed!

## 🤝 Contributing

This is a learning resource designed to grow and improve. Feel free to:
- Suggest new exercises or improvements
- Share your compositions created with these exercises
- Report any errors or unclear explanations
- Add translations or alternative explanations

## 📖 Additional Resources

- [Strudel Documentation](https://strudel.cc/learn/)
- [Strudel Tutorial Videos](https://strudel.cc/learn/getting-started/)
- [Live Coding Community](https://toplap.org/)
- [Music Theory Fundamentals](https://musictheory.net/)

## 🎶 Happy Coding!

Remember: The goal isn't to become a perfect programmer or musician overnight. It's to explore the beautiful intersection of code and music, and discover how algorithmic thinking can enhance musical creativity.

Start simple, be patient with yourself, and most importantly - have fun making music with code!