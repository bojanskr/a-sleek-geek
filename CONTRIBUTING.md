## How to contribute to A Sleek Geek

#### **Did you find a bug?**

* **Do not open up a GitHub issue if the bug is a security vulnerability **, and instead refer to our [security section](https://github.com/bojanskr/a-sleek-geek/).

* **Ensure the bug was not already reported** by searching on GitHub under [Issues](https://github.com/bojanskr/a-sleek-geek/issues).

* If you're unable to find an open issue addressing the problem, [open a new one](https://github.com/bojanskr/a-sleek-geek/issues). Be sure to include
a **title and clear description**, as much relevant information as possible, and a **code sample** 
or an **executable test case** demonstrating the expected behavior that is not occurring.

#### **Did you write a patch that fixes a bug?**

* Open a new GitHub pull request with the patch.
* Ensure the PR description clearly describes the problem and solution. Include the relevant issue number if applicable.
* Before submitting, think about things like the following one.

#### Suggesting Enhancements

This section guides you through submitting an enhancement suggestion for "A Sleek Geek", including completely new features and minor improvements to existing functionality. Following these guidelines helps maintainers and the community understand your suggestion 📝 and find related suggestions 🔎.

Before creating enhancement suggestions, please check [this list](https://github.com/bojanskr/a-sleek-geek/issues) as you might find out that you don't need to create one. When you are creating an enhancement suggestion, please include as many details as possible. Fill in the template, including the steps that you imagine you would take if the feature you're requesting existed.

##### Before Submitting An Enhancement Suggestion

* Check the debugging guide for tips, or the issues list — you might discover that the enhancement is already available. Most importantly, check if you're using the latest version  and if you can get the desired behavior by changing the website's or packages' config settings.
* Check if there's already a package which provides that enhancement.
* Determine which directory the enhancement should be suggested in.
* Perform a cursory search to see if the enhancement has already been suggested. If it has, add a comment to the existing issue instead of opening a new one.

##### How Do I Submit A (Good) Enhancement Suggestion?

Enhancement suggestions are tracked as GitHub issues. After you've determined which repository your enhancement suggestion is related to, create an issue on that repository and provide the following information:

* Use a clear and descriptive title for the issue to identify the suggestion.
* Provide a step-by-step description of the suggested enhancement in as many details as possible.
* Provide specific examples to demonstrate the steps. Include copy/pasteable snippets which you use in those examples, as Markdown code blocks.
* Describe the current behavior and explain which behavior you expected to see instead and why.
* Include screenshots and animated GIFs which help you demonstrate the steps or point out the part of Atom which the suggestion is related to. You can use this tool to record GIFs on macOS and Windows, and this tool or this tool on Linux.
* Explain why this enhancement would be useful to most Atom users and isn't something that can or should be implemented as a community package.
* List some other text editors or applications where this enhancement exists.
* Specify which version of Atom you're using. You can get the exact version by running atom -v in your terminal, or by starting Atom and running the Application: About command from the Command Palette.
* Specify the name and version of the OS you're using.

#### Git Commit Messages

* Use the present tense ("Add feature" not "Added feature")
* Use the imperative mood ("Move cursor to..." not "Moves cursor to...")
* Limit the first line to 72 characters or less
* Reference issues and pull requests liberally after the first line
* When only changing documentation, include `[ci skip]` in the commit title
* Consider starting the commit message with an applicable emoji:
    * :art: `:art:` when improving the format/structure of the code
    * :racehorse: `:racehorse:` when improving performance
    * :non-potable_water: `:non-potable_water:` when plugging memory leaks
    * :memo: `:memo:` when writing docs
    * :penguin: `:penguin:` when fixing something on Linux
    * :apple: `:apple:` when fixing something on macOS
    * :checkered_flag: `:checkered_flag:` when fixing something on Windows
    * :bug: `:bug:` when fixing a bug
    * :fire: `:fire:` when removing code or files
    * :green_heart: `:green_heart:` when fixing the CI build
    * :white_check_mark: `:white_check_mark:` when adding tests
    * :lock: `:lock:` when dealing with security
    * :arrow_up: `:arrow_up:` when upgrading dependencies
    * :arrow_down: `:arrow_down:` when downgrading dependencies
    * :shirt: `:shirt:` when removing linter warnings
    
### Specs Styleguide

- Include thoughtfully-worded, well-structured [Jasmine](https://jasmine.github.io/) specs in the `./spec` folder.
- Treat `describe` as a noun or situation.
- Treat `it` as a statement about state or how an operation changes state.

#### Example

```coffee
describe 'a dog', ->
 it 'barks', ->
 # spec here
 describe 'when the dog is happy', ->
  it 'wags its tail', ->
  # spec here
```

### JavaScript Styleguide

All JavaScript code is linted with [Prettier](https://prettier.io/).

* Prefer the object spread operator (`{...anotherObj}`) to `Object.assign()`
* Inline `export`s with expressions whenever possible
  ```js
  // Use this:
  export default class ClassName {

  }

  // Instead of:
  class ClassName {

  }
  export default ClassName
  ```
* Place requires in the following order:
    * Built in Node Modules (such as `path`)
    * Built in Atom and Electron Modules (such as `atom`, `remote`)
    * Local Modules (using relative paths)
* Place class properties in the following order:
    * Class methods and properties (methods starting with `static`)
    * Instance methods and properties
* [Avoid platform-dependent code](https://flight-manual.atom.io/hacking-atom/sections/cross-platform-compatibility/)

### Documentation Styleguide

* Use [AtomDoc](https://github.com/atom/atomdoc).
* Use [Markdown](https://daringfireball.net/projects/markdown).
* Reference methods and classes in markdown with the custom `{}` notation:
    * Reference classes with `{ClassName}`
    * Reference instance methods with `{ClassName::methodName}`
    * Reference class methods with `{ClassName.methodName}`

#### Example

```coffee
# Public: Disable the package with the given name.
#
# * `name`    The {String} name of the package to disable.
# * `options` (optional) The {Object} with disable options (default: {}):
#   * `trackTime`     A {Boolean}, `true` to track the amount of time taken.
#   * `ignoreErrors`  A {Boolean}, `true` to catch and ignore errors thrown.
# * `callback` The {Function} to call after the package has been disabled.
#
# Returns `undefined`.
disablePackage: (name, options, callback) ->
```

### Notes:

**Did you fix whitespace, format code, or make a purely cosmetic patch?**

**Changes that are cosmetic in nature and do not add anything substantial to the stability, functionality, or testability of Rails will generally not be accepted (read more about [our rationales behind this decision](https://github.com/rails/rails/pull/13771#issuecomment-32746700)).

**Do you intend to add a new feature or change an existing one?**

* Suggest your change in the [Discord](https://discuss.rubyonrails.org/c/rubyonrails-core) and start writing code.

* Do not open an issue on GitHub until you have collected positive feedback about the change. GitHub issues are primarily intended for bug reports and fixes.

**Do you have questions about the source code?**

* Ask any question about how to use Ruby on Rails in the [rubyonrails-talk mailing list](https://discuss.rubyonrails.org/c/rubyonrails-talk).



"A Sleek Geek" is a volunteer effort. We encourage you to pitch in and join [the team](https://www.thebojan.ninja/contributors/)!

Thanks and happy coding! :heart: :heart: :heart:

TehBoyan
