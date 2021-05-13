# EMIKETIC Hygen generators for React, React Native and Gatsby

Hygen generators based on the EMIKETIC React / JavaScript standard.

Meant to be used by EMIKETIC staff but we highly encourage adopt our standard or contribute with new improvement ideas.

## Usage

```
yarn global add hygen-add
```

Or

```
npm i -g hygen-add
```

Then

```
cd your-jsx-project

hygen-add emiketic-react
```

## Command manual

### React Native

---

message: |

    hygen {bold react-native-component new} --feature {bold FEATURE} ---shared {bold TYPE}  --name {bold NAME} {italic [--screen]} {italic [--static]} {italic [--detached]}

    Generates a React Native component, a storybook, and a test all compliant with the EMIKETIC standard.

       NAME           The component name in kebab-case ({bold required}).
       --feature Feature to which belongs the component.
       --shared If not a feature, tells whether this is an atom, molecule or organism.
       --screen  Generate a React Native screen componant (as opposed to composablecomponents).
       --detached Generate a static component that is not connected to store but might have side-effects and API logic.
       --static Generates a static compone not (visual component).

    If no flags given, will generate a non-screen component that is connected to the Redux store.

---

## Generators roadmap

### React Native

- [x] Feature scaffold
- [x] Merges new components in existing features or new features
- [x] Component scaffolds: Screen, static (pure visual), connected (to redux store)
- [x] Style definition
- [x] Storybook story wrapped in app container and covered by storyshot
- [x] Basic Jest unit test
- [ ] Molecules, organisms and atom generation
- [ ] Simple shared components
- [ ] Interactive mode with prompt

### React (_WIP_)

- [ ] Feature scaffold
- [ ] Framework variations (Ex: Ant Design vs. others)
- [ ] Merges new components in existing features or new features
- [ ] Component scaffolds: Pages, Static (pure visual), connected (to redux store)
- [ ] Stylesheet LESS/SCSS definition + responsiveness
- [ ] MDX Storybook story wrapped in app container and covered by storyshot
- [ ] Basic Jest unit test
- [ ] Molecules, organisms and atom generation
- [ ] Simple shared components
- [ ] Interactive mode with prompt

### Gatsby (_WIP_)

- [ ] Page scaffold
- [ ] Component generation (shared or for page)
- [ ] Static localized page
- [ ] Dynamic localized page
