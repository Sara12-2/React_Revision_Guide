# ⚛️ React.js Complete Notes

> A concise, structured guide to understand React.js, its workflow, architecture, and core concepts without long code examples.

---

# 📖 What is React?

React.js is an open-source JavaScript library used to build user interfaces (UI), especially for Single Page Applications (SPAs). It was developed by Meta (Facebook).

React allows developers to create reusable UI components that update efficiently whenever data changes.

---

# 🎯 Why React?

Traditional JavaScript applications become difficult to maintain as they grow.

React solves this by:

- Breaking UI into reusable components
- Updating only changed parts of the page
- Managing application state efficiently
- Making code easier to read and maintain

---

# 🏗 React Architecture

```
Application

│

├── App Component
│
├── Header
│
├── Sidebar
│
├── Main Content
│
├── Cards
│
├── Buttons
│
└── Footer
```

Everything in React is a **Component**.

---

# ⚙ React Working Flow

```
User Action

↓

Event Triggered

↓

State Changes

↓

Virtual DOM Updated

↓

React Compares Changes
(Diffing Algorithm)

↓

Only Changed Elements

↓

Real DOM Updated

↓

Browser Repaints UI
```

This process makes React very fast.

---

# 🌍 Real DOM vs Virtual DOM

## Real DOM

- Browser's actual HTML
- Slow updates
- Entire page may refresh

Example

```
<button>Like</button>
```

Changing button text updates the actual page immediately.

---

## Virtual DOM

A lightweight JavaScript copy of the Real DOM.

Flow:

```
State Changes

↓

Virtual DOM Created

↓

Compare Old vs New

↓

Find Difference

↓

Update Real DOM
```

Only modified elements are updated.

---

# 📦 React Project Structure

```
project/

src/

components/

pages/

assets/

hooks/

App.jsx

main.jsx

public/

package.json
```

---

# 🚀 React Lifecycle

```
Component Created

↓

Rendered

↓

Updated

↓

Destroyed
```

Using Hooks:

- useEffect()

can perform actions during these stages.

---

# ⚛ Components

A component is an independent UI block.

Example:

```
Navbar

Footer

Card

Login Form

Profile

Dashboard
```

Benefits:

- Reusable
- Independent
- Easy to maintain

---

# 🧩 Types of Components

### Functional Component

Modern approach.

Uses Hooks.

### Class Component

Older approach.

Uses lifecycle methods.

Mostly replaced by Functional Components.

---

# 📨 Props

Props transfer data from parent to child.

Flow

```
Parent

↓

Props

↓

Child
```

Properties are read-only.

---

# 💾 State

State stores changing data.

Example:

```
Counter

Cart Items

Dark Mode

Login Status
```

Flow

```
User Click

↓

State Changes

↓

Component Re-renders

↓

UI Updates
```

---

# 🔄 React Rendering Flow

```
Component

↓

JSX

↓

Virtual DOM

↓

Compare

↓

Real DOM

↓

Screen
```

---

# 📄 JSX

JSX = JavaScript XML

Allows writing HTML inside JavaScript.

React converts JSX into JavaScript before running.

---

# 📢 Event Handling

Events respond to user actions.

Examples:

- Click
- Hover
- Submit
- Change
- Focus

Flow

```
User Click

↓

Event

↓

Function Executes

↓

State Updates

↓

UI Updates
```

---

# 🔀 Conditional Rendering

React can display different UI depending on conditions.

Example situations

- Logged In
- Loading
- Error
- Admin Panel

Flow

```
Condition

↓

True

↓

Show Component

Else

↓

Show Another Component
```

---

# 📋 Lists

React displays arrays using loops.

Flow

```
Array

↓

Loop

↓

Component

↓

Display List
```

Each item should have a unique Key.

---

# 📝 Forms

Forms collect user input.

Examples

- Login
- Registration
- Contact Form

Flow

```
Input

↓

State

↓

Validation

↓

Submit

↓

Server
```

---

# 🎣 React Hooks

Hooks allow Functional Components to use React features.

---

## useState

Purpose

Stores dynamic data.

Examples

- Counter
- Input
- Theme

---

## useEffect

Purpose

Handles side effects.

Examples

- API Calls
- Timers
- Local Storage
- Event Listeners

Flow

```
Component Loads

↓

useEffect Runs

↓

Task Executes
```

---

## useRef

Purpose

Stores values without re-rendering.

Used for:

- Input Focus
- DOM Access
- Timers

---

## useContext

Purpose

Share data globally.

Example

```
Theme

↓

Context

↓

All Components
```

No need for prop drilling.

---

## useMemo

Purpose

Stores expensive calculations.

Improves performance.

---

## useCallback

Purpose

Stores functions.

Prevents unnecessary recreation.

---

# 🌐 Routing

Allows navigation without page reload.

Example

```
Home

↓

About

↓

Products

↓

Contact
```

Flow

```
URL Changes

↓

Router

↓

Component

↓

Display Page
```

---

# 🌍 API Integration

React communicates with backend services.

Flow

```
Component

↓

API Request

↓

Server

↓

Response

↓

State Updates

↓

UI
```

Common methods

- GET
- POST
- PUT
- DELETE

---

# 🎨 Styling

Methods

- CSS
- CSS Modules
- Tailwind CSS
- Styled Components

---

# 📁 Recommended Folder Structure

```
src/

components/

pages/

hooks/

context/

services/

utils/

styles/

assets/

routes/

layouts/
```

---

# ⚡ React Performance

React is fast because of

- Virtual DOM
- Component Reuse
- Memoization
- Lazy Loading
- Code Splitting

---

# 🔐 Data Flow

React follows One-Way Data Flow.

```
Parent

↓

Child

↓

Grand Child
```

Child cannot directly change Parent data.

---

# 📈 Complete React Flow

```
User Opens Website

↓

React Loads

↓

App Component

↓

Child Components

↓

JSX

↓

Virtual DOM

↓

Browser

↓

User Clicks Button

↓

State Changes

↓

Virtual DOM Updates

↓

Diffing

↓

Real DOM Updates

↓

Screen Refreshes
```

---

# 📚 Common React Terms

| Term | Meaning |
|------|----------|
| JSX | HTML inside JavaScript |
| Component | Reusable UI Block |
| Props | Parent → Child Data |
| State | Dynamic Data |
| Hook | React Feature Function |
| Virtual DOM | Copy of Real DOM |
| Rendering | Display UI |
| Re-render | Update UI |
| Context | Global State |
| Router | Page Navigation |

---

# ⭐ Advantages

- Fast rendering
- Reusable components
- Easy maintenance
- Huge ecosystem
- SEO support (with Next.js)
- Large community
- Cross-platform (React Native)

---

# ❌ Limitations

- Only handles the UI layer
- Requires additional libraries for routing and state management
- Frequent ecosystem changes
- JSX may feel unfamiliar to beginners

---

# 🎯 React Learning Roadmap

```
HTML
↓

CSS
↓

JavaScript ES6
↓

React Basics
↓

Components
↓

Props
↓

State
↓

Events
↓

Hooks
↓

Routing
↓

API Calls
↓

State Management
↓

Authentication
↓

Performance
↓

Testing
↓

Next.js
```

---

# 🏁 Summary

React is a component-based JavaScript library that builds fast, dynamic, and interactive user interfaces. Its workflow revolves around components, state, props, hooks, and the Virtual DOM, ensuring that only necessary UI updates are rendered. Understanding these core concepts provides the foundation for building scalable and maintainable web applications.
