# Dr. Felicity Leonard DVM

A three-page Jekyll site with Home, Contact, and Handouts pages. Contact details
are editable in `_data/site.yml`; handout files and their listing information
are maintained separately.

## Run locally

Install Jekyll and Bundler, then run:

```sh
bundle exec jekyll serve
```

If you do not have a Gemfile yet, install Jekyll and run `jekyll serve` instead.
Open the local URL printed by Jekyll, usually `http://127.0.0.1:4000`.

## Edit the site

- Update the contact details and image URLs in `_data/site.yml`. Replace the
    contact placeholders before publishing.
- To add a handout, upload its file into `assets/handouts/`, then add an entry
    to `_data/handouts.yml` with its name, description, and path:

    ```yaml
    - name: Visit preparation guide
        description: What to bring and expect at your pet's appointment.
        file: /assets/handouts/visit-preparation-guide.pdf
    ```

- Delete a handout by removing its entry from `_data/handouts.yml` and its file
    from `assets/handouts/`.
