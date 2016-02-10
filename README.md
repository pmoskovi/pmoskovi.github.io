# KWIC Microsite

## Running the Microsite locally for testing

0. Clone or fork the repo locally.

0. In the top level directory, start a HTTP server that can serve from files in place. For example:
    * Using Jekyll:

        `$ jekyll serve --watch --port 4000`

    * Using Python:

        `$ python -m SimpleHTTPServer 4000`

0. Using a browser, go to [http://localhost:4000/kwic/](http://localhost:4000/kwic/)

## Deploying the Microsite to kaazing.com

Deployment happens auto-magically, using github webhooks.
Steps to set up webhooks (needs to be done by dev-ops, only once):

0. Navigate to [https://github.com/kaazing/corporate/](https://github.com/kaazing/corporate/).

0. Click **Settings** on the right hand side.

0. Select **Webhooks & Services** on the left.

0. Click **Add webhook**.

0. In the **Payload URL** field enter `http://www-stage.kaazing.com/wordpress/update-kwic-site.php`.

0. Click **Add webhook**.

0. Repeat the above steps for the production environment.