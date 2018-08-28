swagger: "2.0"
x-collection-name: Heroku
x-complete: 1
info:
  title: Heroku
  description: manage-your-heroku-apps-configs-collaborators--resources
  version: "1"
host: api.heroku.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /apps/{app}/ps:
    post:
      summary: Add Application PS
      description: Run a one-off process.
      operationId: postAppsAppPs
      x-api-path-slug: appsappps-post
      parameters:
      - in: header
        name: Accept
        description: Content type
      - in: query
        name: Accept
        description: Content type
      - in: query
        name: app
        description: The app name
      - in: path
        name: app
      - in: query
        name: attach
        description: 'true: use rendezvous to access stdin/stdout - : stream process
          output to the application log'
      - in: query
        name: command
        description: The command to run
      responses:
        200:
          description: OK
      tags:
      - Application
      - PS