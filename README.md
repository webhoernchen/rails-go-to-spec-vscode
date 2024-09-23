# Rails Go to Spec V3 extension for VSCODE

Jump between code and spec in Rails projects.

To install search for

```
rails-go-to-spec-v3
```

The difference with the original version is that this version supports the "search" for test files when we use the convention:

```ruby
# path public/some_service.rb
module SomeService
  extend self

  def method_name
	# ...
  end
end

# path spec/some_service/method_name_spec.rb
describe SomeService, "#method_name" do
end
```



## Default keybinding:

- Ctrl + Shift + y
- Cmd + Shift + y (Mac)

## Redine shortcuts:

In keybindings.json

```
  ...
	{
		"key": "shift-cmd-y",
		"command": "rails-go-to-spec-v3.railsGoToSpec",
		"when": "editorFocus"
	}
	...
```
