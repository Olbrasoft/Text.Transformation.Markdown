Text.Transformation.Markdown
=======
[![NuGet](https://img.shields.io/nuget/vpre/Olbrasoft.Text.Transformation.Markdown.svg)](https://www.nuget.org/packages/Olbrasoft.Text.Transformation.Markdown/)

Interface IMarkdownTransformer and Implementation MarkdownTransformer dependent on Markdown and AgilityPack and MarkdownTagHelper

1. Instal-Package  Olbrasoft.Text.Transformation.Markdown

2. Edit `Startup.cs` 

```diff
 public void ConfigureServices(IServiceCollection services)
 {
   services.AddTextTransformationMarkdown()
```

3. Edit `_ViewImports.cshtml`

```diff
@addTagHelper *, Microsoft.AspNetCore.Mvc.TagHelpers
+ @addTagHelper *, Olbrasoft.Text.Transformation.Markdown
```

## Usage
```html
<markdown raw="true">**AnyStringMarkdown**</markdown>
```

![Olbrasoft markdown transformation](./olbrasoft-text-transformation-markdown.png)