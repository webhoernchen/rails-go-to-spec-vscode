# Rails Go to Spec V3 extension for VSCODE

Jump between code and spec in Rails projects.

To install search for

```
rails-go-to-spec-v3
```

The difference with the original version is that this extension allows you to ‘Go to Spec’ when have a service, and for each method of the service, there is a different spec file.

For example:

```ruby
# public/some_service.rb
module SomeService
  extend self

  def method_name_1
    # ...
  end

  def method_name_2
    # ...
  end
end

# public/spec/some_service/method_name_1_spec.rb
describe SomeService, "#method_name_1" do
  # ...
end

# public/spec/some_service/method_name_2_spec.rb
describe SomeService, "#method_name_2" do
  # ...
end
```

**IMPORTANT 👀:**
To make it to work
 - You need to place the cursor on the method name.
 - The service must be in the `/public/` folder
 
## Default keybinding:

- Ctrl + Shift + y
- Cmd + Shift + y (Mac)

## Redine shortcuts:

In keybindings.json

```json
...
{
  "key": "shift-cmd-y",
  "command": "rails-go-to-spec-v3.railsGoToSpec",
  "when": "editorFocus"
}
...
```
