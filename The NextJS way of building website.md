# The NextJS way of building website



- NextJS is a React Framework for building web application. NextJS comes out-of-the-box with Prerendering in the form of server-side rendering and  static site rendering although client-side rendering is possible. Since prerenders is used we can significant improve SEO as we can inject all kinds of tags into the webpage that is rendered to the client.
- Since NextJS offers two ways of prerendering (SSR or Static rendering) we have to choose which types to render webpages, hence most of the website built with NextJS is in hybrid mode where both rendering techniques are used. The rule of thumb when choosing rendering technique is to answer the question "Can I pre-render this page ahead of user request ?", if the answer is yes then choose static rendering technique, otherwise choose SSR. 







