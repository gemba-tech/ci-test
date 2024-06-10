# create feature

- gh issue develop <issue #> -b main -c -n feature/<issue #>-<feature name>
- git add -A .
- git commit -am <message>
    - triggers commit-msg
- git push -u origin
- gh pr create --draft --fill -B main
    - git commit -am <message>
        - triggers commit-msg
    - git push -u origin
- gh pr ready 
- gh pr edit --add-reviewer <reviewer name>
- gh pr review --request-changes --body <message>
- gh pr review --approve --body <message>

- git checkout -b feature/[issue #]-<feature_name> -t origin feature/[issue #]-<feature_name>
- gh pr create --fill -B main

