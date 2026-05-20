# DNA

## Hard Constraints & Rules
1. **Svelte Best Practices**:
   - Use Svelte's native reactivity model correctly (e.g., use `$: double = count * 2` for derived values).
   - Utilize Svelte stores (`writable`, `readable`, `derived`) for global state, always clean up subscriptions or use the `$` auto-subscription syntax.
   - Ensure proper use of Svelte transition and animation directives (`transition:fade`, `animate:flip`) for smooth UX.
2. **Tailwind Best Practices**:
   - Avoid writing custom CSS in `<style>` tags unless absolutely necessary (e.g., highly complex dynamic calculations that cannot be solved with Tailwind classes or CSS variables).
   - Leverage Tailwind's arbitrary values (e.g., `h-[400px]`) sparingly; favor the design system configuration.
   - Group classes logically (e.g., layout -> spacing -> sizing -> typography -> colors -> interactive states).
3. **TypeScript Integration**: Write type-safe code using TypeScript within Svelte components (`<script lang="ts">`).