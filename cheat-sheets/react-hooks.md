# Cheat sheet: React Hooks

Ce fichier est là pour vous donner un aperçu des hooks que vous pourriez utiliser dans vos composants.

- [Cheat sheet: React Hooks](#cheat-sheet-react-hooks)
  - [useState](#usestate)
    - [update state](#update-state)
  - [useEffect](#useeffect)
  - [useContext](#usecontext)


## [useState](https://react.dev/reference/react/useState)
Permet de gérer l'état d'un composant.
```jsx
import React, { useState } from 'react';

// ...

const [state, setState] = useState(initialState);
```

### update state
```jsx
setState(newValue);
```

## [useEffect](https://react.dev/reference/react/useEffect)
```jsx
import React, { useEffect } from 'react';

// ...

useEffect(() => {
  // code à exécuter
}, [dependencies]);
```

Le code sera exécuté à chaque fois que les dépendances changent.

> Pro tip: Si vous ne mettez pas de dépendances, le code sera exécuté à chaque rendu.
> Pro tip: Attention lorsque la dépendance est un objet.

## [useContext](https://react.dev/reference/react/useContext)
```jsx
import { useContext } from 'react';

const MyComponent = () => {
  const theme = useContext(ThemeContext);
  // ...
}

```

```jsx
const MyPage = () => {
  return (
    <ThemeContext.Provider value="dark">
      <Form />
    </ThemeContext.Provider>
  );
}
```