# eScience Conference Series Website Template

This is a template for the eScience conferece websites. To start using this template, please **fork** this repository into a new repository at the [escience-conference](https://github.com/escience-conference) GitHub organization in which the repository name should be the year of the conference (e.g., `2022`).

## Customizing the website

Once forked, there are a few steps that need to be followed to properly configure the website.

### Configuration file

In `config.yml`, edit the line `baseurl: /_template` with the conference year (e.g., `baseurl: /2022`)

### Conference information

In `_data/main.yml`, edit the `edition`, `dates`, `location`, and `description` keys with the current's year conference information.

### Contents visibility

In `_data/main.yml`, the `contents` key controls which pages/links will be **visible** in the website menu. If you want to hide (resp. display) a menu option, use `false` (resp. `true`) as value for the sub-keys.

### Important dates

Edit `_data/important_dates.yml` with the list of important events (e.g., deadlines, notifications, etc.) related to the conference:

- `type` and `date` are required keys
- If the `extended` key is used, it will strikethrough the original date text and display the extended date instead
- Important dates will be displayed in the order entered in the file

### Organizers

Edit `_data/organizers.yml` with the list of organizers:

- `name`, `role`, and `institution` are required keys
- Possible values for `role` include: `General Chair`, `Program Chair`, `Publication Chair`, `Publicity and Web Chair`, `Workshop Chair`, `Tutorial Chair`, `Poster Chair`, `Local Chair`, `Industry Chair`, and `Finance Chair`
- `photo` is an optional key that if provided an image file must be placed into `/images/organizers`
