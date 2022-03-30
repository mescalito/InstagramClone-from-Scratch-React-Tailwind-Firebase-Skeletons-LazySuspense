# Instagram from Scratch with  React, Tailwind CSS, Firebase
<img src="https://raw.githubusercontent.com/mescalito/BIG_React_App_tailwind_skeleton_lazy_suspense_Firebase/master/instagram-preview.png">

# 📣 Summary

This application (Instagram clone) was built using React (Custom Hooks, Context), Firebase & Tailwind CSS. I have built the following pages within this application: login, sign up, dashboard & lastly the user profile page. There are four different pages, some are public and some are private with auth listeners. Firebase firestore handles all the data, and that data is retrieved using a custom hook.

I used Tailwind CSS for this project and I really enjoyed using it.

# Code info
### React hooks in use:
  - useRef
  - useContext
  - createContext
  - useHistory
  - useState
  - useReducer
  - useEffect
  - Custom hooks:
    - useUser
    - usePhoto
  - Webpack
### Libs
  - skeleton
  - lazy
  - Suspense
  - firebase
  - tailwindcss
  - prop-type
  - react-router-dom
    - useHistory
    - Link
    - useParams
  - date-fns
  - react-loader-spinner: nice to have
  - react-loading-skeleton
  - eslint
  - prettier
  - ESLINT by airbnb
  - Chrome Console: Rendering > Core Web Vitals
  - CONSTs for routing
  - Link from react-router-dom: \<Link to={ROUTES.SIGN_UP}>Sign up\</Link>
  - Uses localStorage to save user data coming from Firebase
    - Listener to update user data when auth changes
  - Custome hooks:
    - use:User
    - usePhotos
  - Tailwind:
    - grid-cols-3
      - 1024
        - 2/3 <-> 1/3
        - 66% | 33%
  - Uses Skeletons to improve UX
  - NPM paquete "loadtest" ayuda a probar cuandor rps request per second puede mantener la aplicacion

# features
- Login page: As a user I want the submit button to be disabled if fields are empty or dirty
- Login page: As a user I want to submit the form only when password contains more than 3 characters
- As a user, I want to receive only the chunks needed to render the page and anything else (lazy/suspense & chunks (webpack))
- Pictures: As a user, I want to comment other's people pictures
- Pictures: As a user, I want to use the enter key to focus on the comment (useRef())
- Pictures: As a user, I want to see a maximum of 3 comments per picture and then wrap the rest of comments
- Pictures: As a user, I want to see how old are the comments (useRef())
- Pictures: As a user, I want to like/unlike a picture
- Pictures: As a user, I want to see how many likes and comments has a picture
- User Activity: As a user, I want to follow or unfollow a user
- TimeLine: As a user, I want to have my own picture gallery page profile
- TimeLine: As a user, I want to have a list of user I follow
- TimeLine: As a user, I want to have restricted pages I can't visit if my auth doesn't allow it (/dashboard)
- TimeLine: As a user, I want to get a warning if I try to register the same user multiple times
- TimeLine: As a user, I want to have a timeline containing all the pictures from all the users
- NavBar: As a user, I want have a button to log out after login.
- NavBar: As a user, I want to use the keyboard to log out (onKeyDown)
- NavBar: As a user, I want to have an avatar with my picture
- NavBar: As a user, I want to go to my picture's gallery when clicking my avatar
- NavBar: As a user, I want all icons to be SVGs
- As a user, I want to see a loader while the items are loaded to avoid an empty page (SKELETON)
- As a user, I want to get redirected to my Timeline if I try to access the login or sing up route to improve UX
- As a user, I want to stay loged in after I close the browser and come back



# To Improve
- Crear una CONSTANTE que determine cuantos comentarios se muestran por fafault por foto, actualmente se muestran 3 (compnents/post/comments)
- crear un debaunce en el login page cuando se esta llenando el email de autenticacion para q no se haga render cada vez q se escribe algo en el input
- Cuando un usuario autenticado en el sistema intenta navegar a un route como /login lo redirecciona al dashboard, ya q no hay necesidad de mostrarle /login

# comandos
``` shell

yarn start

npx create-react-app instagram

Extra modulos:
yarn add date-fns
yarn add firebase
yarn add react-loading-skeleton

==================

eslint:
npx install-peerdeps --dev eslint-config-airbnb
yarn add @babel/preset-react -D
Configure Babel
.babelrc file in the project root:

{
    "presets": [
        "@babel/preset-react"
    ]
}

============

yarn add react-router-dom

```
