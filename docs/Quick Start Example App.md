## Quick Start Example App

> Build once, render anywhere.
> OBIUI doesn’t care *how* you model — only *why*.

OBIUI works across environments — web, mobile, desktop, or assistive devices — by focusing on **intention**, not implementation details.

### 📱 Minimal, Mobile-First Example

```tsx
import { Interface, Section, Action, Text, Input } from '@obinexus/obiui';

export default function QuickStartApp() {
  return (
    <Interface
      respects="user-accessibility"
      adapts="mobile-first"
      honors="minimalism"
    >
      <Section intent="onboard">
        <Text variant="headline">Welcome to OBIUI</Text>
        <Text variant="body">
          A place where design leads with intention — not framework.
        </Text>

        <Input
          label="Your name"
          placeholder="Type here..."
          inputMode="text"
          accessibilityLabel="Name input field"
        />

        <Action
          intent="primary"
          ariaLabel="Continue"
          onPress={() => alert('Hello, human heart.')}
        >
          Continue
        </Action>
      </Section>
    </Interface>
  );
}
```

### 🧭 Notes

* **Model-agnostic:** Works conceptually in React, Svelte, Vue, Flutter, or plain HTML — the pattern stays the same.
* **Mobile-first:** All layout, spacing, and interaction scales *up* from handheld dimensions.
* **Accessible defaults:** Every component ships with ARIA mappings, contrast-safe theming, and haptic-aware feedback.
* **Intention-driven:** Components describe *why they exist*, not *how they render*.

### 🪶 Structure Summary

```
Interface      → the living container of user intent
 ├─ Section    → logical flow, often task-based
 │   ├─ Text   → communicates meaning and tone
 │   ├─ Input  → receives the user’s voice
 │   └─ Action → responds with respect
```

### 🧘‍♀️ Principle

Design is not presentation.
Meaning is not styling.
The interface *breathes* where intent meets access.
