# programming-notes

```css
/* flex justify-center items-center */
/* flex flex-col justify-between */

@keyframes blink {
  0% {opacity: 0;}
  50% {opacity: 1;}
  100% {opacity: 0;}
}
.blink {
  animation: blink 2s infinite;
}

```

even `text-gray-600` makes `hover:text-primary-600` un-inheritable

GraphQL will return status code of 400 if the query is invalid. Otherwise it will always return status code of 200 even if an Error is thrown in resolver. Which can be accessed with Apollo {error}. Callback's don't work with GraphQL resolver functions.

if height or width is not defined explicitly border-box have no use

it is correct to call 'returns promise'. 

GraphQL queries are stored in client's in-memory cache, so future requests for same data will be served from cache. Which also means mutations should update that cache \(logout was also a problem\). 

Apollo fetch policies - [https://www.apollographql.com/docs/react/data/queries/\#supported-fetch-policies](https://www.apollographql.com/docs/react/data/queries/#supported-fetch-policies).

?? \(nullish coalescing operator\) \(null \|\| undefined\) ?? 'this will print'.

tracking-wider \(css letter-spacing\) to increase or decrease letter spacing.

Google OAuth does not have test mode so we can easily use it in localhost & production without changing anything. 

Facebook OAuth have test mode and if it is Live we have to connect with HTTPS in localhost in order to test Facebook OAuth.

e =&gt; e.stopPropagation\(\) // stops further propagation of the current event. Could mean parent's on click won't get triggered on child's element click.

```markup
<link rel="alternate" hreflang="lang_code" href="url_of_page" />
<!-- example -->
<link rel="alternate" href="https://resume.io/" hreflang="en">
<link rel="alternate" href="https://cvapp.fr/" hreflang="fr-FR">
<link rel="alternate" href="https://cvster.nl/" hreflang="nl-NL">
<link rel="alternate" href="https://cvapp.es/" hreflang="es-ES">
<link rel="alternate" href="https://cvapp.fi/" hreflang="fi">
<link rel="alternate" href="https://cv.dk/" hreflang="da">

<!-- https://support.google.com/webmasters/answer/189077
even Google & Amazon does it like:
google.com
google.com.tr
So different domains should be the way to go -->

```

onKeyDown with e.key \(gives string values of key pressed for focused inputs\) for input components, if a key changes on re-render input will lose focus.

while using useMemo, props are passed in but it does not re-render.

If a mapped components are going to change order or inserted & deleted, don't use array's index as key. That will force react to re-render all of the components that's key changed. [https://github.com/yannickcr/eslint-plugin-react/blob/master/docs/rules/no-array-index-key.md](https://github.com/yannickcr/eslint-plugin-react/blob/master/docs/rules/no-array-index-key.md)

Fallback weights: [https://developer.mozilla.org/en-US/docs/Web/CSS/font-weight\#fallback\_weights](https://developer.mozilla.org/en-US/docs/Web/CSS/font-weight#fallback_weights) if a given weight is not found font weight will be changed to what ever closest available \(exact details in the link\).

in order to align middle absolutely positioned elements, `inset-y-0 flex items-center` \(makes the element's h full relative to relative element\).

