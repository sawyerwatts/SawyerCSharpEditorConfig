# Sawyer's EditorConfig

 This repo builds off the `dotnet new editorconfig` to contain changes subject
 to my preferences.

## Installation

Here are the steps in bash:

```sh
template_dir=~/.dotnetTemplates/SawyerCSharpEditorConfig
git clone https://github.com/sawyerwatts/SawyerCSharpEditorConfig.git $template_dir
rm -rf $template_dir/.git
rm $template_dir/.gitignore
rm $template_dir/README.md
rm $template_dir/LICENSE
dotnet new install $template_dir
```

Here are the steps in PowerShell:

```ps1
$templateDir="$env:USERPROFILE\.dotnetTemplates\SawyerCSharpEditorConfig"
git clone https://github.com/sawyerwatts/SawyerCSharpEditorConfig.git $templateDir
rm $templateDir\.git -r -force
rm $templateDir\.gitignore
rm $templateDir\README.md
rm $templateDir\LICENSE
dotnet new install $templateDir
```

## Uninstallation

Here are the steps in bash:

```sh
template_dir=~/.dotnetTemplates/SawyerCSharpEditorConfig
dotnet new uninstall $template_dir
rm -rf $template_dir
```

Here are the steps in PowerShell:

```ps1
$templateDir="$env:USERPROFILE\.dotnetTemplates\SawyerCSharpEditorConfig"
dotnet new uninstall $templateDir
rm $templateDir -r -force
```

## Features

1. Most notably, member naming conventions are upgraded from suggestions to
warnings.

