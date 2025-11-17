# Time-Based Animation Project

## Project Overview
A dynamic time-based animation inspired by Pacita Abad's "Wheels of Fortune," featuring 15 animated wheels with pulsating chains and rhythmic transformations driven entirely by time.

## Instructions for Interaction

**How to Experience the Animation:**
1. **Simply load the page** - Open `index.html` in a web browser
2. **Watch and observe** - No user input required
3. **Notice the patterns** - The animation creates its own rhythm:
   - Wheels rotate at different speeds
   - Chains expand and contract rhythmically
   - Colors shift between warm and cool palettes
   - Additional shapes float around the composition

**No interaction needed** - This is a self-contained temporal experience that evolves automatically.

## Individual Animation Approach

**Chosen Driver: TIME**

I selected time as the primary driver to create a predictable, rhythmic animation that feels like a visual clock or musical composition.

## Animated Properties & Unique Features

**Animated Elements:**
1. **Rotation** - Each wheel spins at unique, time-varying speeds
2. **Pulsation** - Chains breathe in and out with smooth oscillations
3. **Color Transitions** - Background and elements shift between color schemes
4. **Scale Variations** - Gentle size pulsations create organic movement
5. **Orbital Elements** - Floating shapes move in circular patterns
6. **Phase Changes** - Different behaviors activate in 5-second intervals

**What Makes This Unique:**
- Focuses on **movement and transformation** rather than static beauty
- Uses **predictable time patterns** instead of random noise
- Creates a **self-contained world** that doesn't require user interaction
- Emphasizes **rhythmic harmony** between all elements

## Technical Implementation

**Core Animation System:**
```javascript
// Time drives all transformations
animationTimer += 0.016; // Continuous time progression

// Smooth oscillations using trigonometric functions
wheel.rotation += speed * time;
wheel.wobble = Math.sin(animationTimer * frequency) * amplitude;
```

**Key Technical Features:**
- **60fps continuous rendering** for smooth animation
- **Phase-based state management** (changes every 5 seconds)
- **Individualized motion parameters** for each wheel
- **Layered animations** that compound naturally
- **Trigonometric functions** for organic movement

## Modifications from Group Code

**Major Changes:**
1. **Real-time Animation** - Converted from static to continuous `draw()` loop
2. **Time Variables** - Added `animationTimer`, `rotationSpeeds`, `pulseFactors`
3. **Dynamic Elements** - Made chains and wheels responsive to time
4. **Enhanced Visuals** - Added floating shapes and background effects
5. **State Management** - Implemented phase-based behavior changes

**Preserved Group Elements:**
- All original wheel positions and color schemes
- Core drawing functions and patterns
- Chain generation algorithm
- Wheel variant decorations (A, B, C types)

## Inspiration & References

**Primary Inspiration: Clock Mechanisms**
The predictable, interlocking movements of clock gears influenced the connected wheel rotations and rhythmic patterns.

**Visual Inspiration: Kinetic Art**
Artists like George Rickey and Alexander Calder inspired the balanced, rhythmic movements and organic transformations.

**Technical References:**
- p5.js trigonometric functions for smooth motion
- Time-based animation patterns from game development
- Phase systems from interactive installations

## How to Run

1. **Open in VS Code** - Create a folder and add all files
2. **Launch** - Right-click `index.html` and select "Open with Live Server"
3. **View** - Alternatively, open `index.html` directly in any web browser

## File Structure
```
project-folder/

- index.html          # Main HTML file
- sketch.js           # Primary animation code
- style.css           # Styling
- jsconfig.json       # JavaScript configuration
- README.md           # This file
```

## Requirements
- Modern web browser with JavaScript enabled
- Internet connection (for p5.js CDN)

The result is a living composition where time acts as the invisible artist, continuously transforming Pacita Abad's vibrant visual foundation into an ever-evolving dance of color and motion.