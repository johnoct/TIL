<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
**Table of Contents**  *generated with [DocToc](https://github.com/thlorenz/doctoc)*

- [reset-input-form-value](#reset-input-form-value)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

# reset-input-form-value

TIL I can reset the input of my form element.

I had some trouble resetting an text input value during one of my exercises.
The key was to reset the element target.

```
e.target.reset();
```

Here's some context:
```
class AddOption extends React.Component {
    ...
    ...
    handleAddOption(e) {
        e.preventDefault();
        /* 
        Some Logic Here
        */
        e.target.reset();
    }
    render() {
        return (
            <div>
                <form onSubmit={this.handleAddOption}>
                    <input name='option' type='text' />
                    <button>Add Option</button>
                </form>
            </div>
        )
    }
}
```