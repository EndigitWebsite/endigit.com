# Endigit.com Website Generation

## Directory Structure

 - /
   - Config files and the sorts
   - source/
     - Everything here gets copied directly to the final build save the following
     - *.haml files: Are converted to HTML
     - layouts/
       - Only used by other .haml files
     - stylesheets/
       - *.scss files are converted to .css files
     - javascripts/
       - *.js files will be built using the sprockets trees

## Previewing Changes

### c9.io
Open the `server.sh` file and click the `Run` button on the c9 IDE.
Click the `Preview` button, and `Preview Running App` to see the preview or get
the URL for sharing/testing.

### Other
In a terminal run `middleman` and the preview will be available at
`http://localhost:4567/`

## Deploying
In a terminal run `middleman deploy` and then just wait. This will build all the
static files, and do a git push to the endigit github pages repo, and the
production site will be updated shortly afterwards.