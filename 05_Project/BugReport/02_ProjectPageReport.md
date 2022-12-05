## Summary (Summarize the bug encountered concisely)

    When signed in to account and clicking "New project" from "Project" page,
    user is then shown "Create **black** project" instead of "Create **blank** project".

    URL where to problem occurs: https://gitlab.com/projects/new

## Steps to reproduce

    Open Browser
    Navigate to https://gitlab.com/users/sign_in
    Log in to account
    Land to "Projects" page
    Click button "New Project"

## What is the current bug behavior?

    When user clicks "New Project" from "Project" page, text "Create **black** project" is shown for creating a new blank project.

## What is the expected correct behavior?

    When user clicks "New Project" from "Project" page, text "Create **blank** project" should be shown for creating a new blank project.

## Relevant logs and/or screenshots

    ### Example image of the bug

![bug]

[bug]: Image/Bug_Project_create_blank.png

## Possible fixes

    <h3 class="gl-font-size-h2 gl-reset-color">
            Create black project
          </h3>

    Above code has typo in it. Change "black" to "blank".

## Whom do you report/ Assign To/ Tags

    /label ~bug ~typo ~easy-to-fix /cc @testing-project-05-manager /
    assign @qa-tester

## Priority

    The severity of the bug is **low**. The bug doesn't hinder the systems
    processes, and thus it is given priority of **Minor**.
