# React Final Project

## Description

This is your final React project. It is an **individual** project. **You choose what to build** — the theme is yours, but the technical requirements are fixed and everyone is graded against the same checklist below.

This is a **frontend-only** project. There is no backend — your data comes from one of the **free public APIs** listed below, or from a local **JSON file** you import (see the note under the API list).

Your finished app must be **hosted online**. You will submit your live URL through a **Google Form** (the link will be shared with you).

## Pick a Theme

Choose one, or propose your own (get it approved first):

1. **Food ordering app** — browse dishes, detail page, cart, checkout confirmation.
2. **E-commerce storefront** — products with search/filters, detail page, cart.
3. **Movie / TV show explorer** — browse and search shows, detail page, "My List" favorites.
4. **Recipe finder** — search recipes, view details, save favorites.
5. **Pokédex / character encyclopedia** — browse, search, details, favorites team.

Whatever the theme, your app must have the same shape: **browse → detail → save/cart → review**.

## Requirements Checklist

### React Fundamentals

- [ ] Built with **Vite + React**
- [ ] Broken into **reusable components** (Header, Footer, Card, etc.)
- [ ] **`useState`** for interactive UI (forms, filters, quantity, toggles)
- [ ] **`useEffect`** used correctly (loading data on mount, proper dependency array)

### Routing (React Router)

- [ ] At least **4 pages**: Home, Browse/List, Detail with a **URL parameter** (e.g. `/products/:id`), and Cart/Favorites
- [ ] A **404 page** for unknown routes
- [ ] Navigation through a shared **Header** (no full page reloads)

### Browse / List Page

- [ ] **Filters** to filter through your items (category, price, type, etc.)
- [ ] **Pagination** (client-side is fine)

### Context

- [ ] A **Context** (cart or favorites) shared across pages: add from the detail page, count badge in the Header updates, view/remove on the cart page
- [ ] Context state **persists on refresh** via `localStorage`

Note: passing props from page to page does not count as Context. The provider must wrap your routes and at least two pages must consume it.

### Hosting & Submission

- [ ] Deployed and **publicly accessible** (Netlify or Vercel)
- [ ] Refreshing on any route (e.g. `/products/3`) does **not** break the app
- [ ] Live URL submitted through the **Google Form**

### Bonus Features (extra credit)

- [ ] At least **one `fetch` call to a live public API**, with a **loading state** while fetching and an **error state** if it fails
- [ ] **Add to favorites** — a second saved list (favorites/wishlist) alongside your main cart/list

## Free Public APIs (no key required)

| API | Good for | URL |
| --- | --- | --- |
| DummyJSON | Products, carts, recipes | https://dummyjson.com |
| Fake Store API | E-commerce products | https://fakestoreapi.com |
| TheMealDB | Recipes / food | https://www.themealdb.com/api.php |
| TheCocktailDB | Drinks menu | https://www.thecocktaildb.com/api.php |
| TVMaze | TV shows + search | https://www.tvmaze.com/api |
| PokéAPI | Pokémon | https://pokeapi.co |

**Note:** some APIs don't provide images or enough detail. In that case you can store your items/products in a local **JSON file** and import it as your app's data — just make sure each item has relevant meta information (category, price, tags, etc.) so your filters have something to filter on.

## Hosting

Deploy with **Netlify** or **Vercel** (both free). Figuring out how to deploy is part of the project.

Deploy early — don't leave hosting for the last hour.

## Suggested Build Order

1. Pick theme + data source (API or JSON file). Scaffold Vite, set up routes and page shells, Header/Footer, list page rendering real data.
2. Filters and pagination on the list page. Detail page with URL params and interactive state (quantity, options).
3. Context: provider, header badge, cart/favorites page with add/remove, `localStorage`.
4. 404 page, styling polish, bonus features, deploy, submit the form.

## Rules

- This is an **individual** project.
- No backend, database, or auth — frontend only.
- Functionality first, styling last.
- There is no presentation for this project. **However: do not just copy and paste from AI. Understand what you are building and how it works — this matters.**

## Grading

| Area | Weight |
| --- | --- |
| Context (working across pages) | 35% |
| Routing + pages | 25% |
| Component structure & state (filters, pagination) | 20% |
| Hosted, working, submitted correctly | 20% |
| Bonus (live API call, favorites) | up to +10% |
