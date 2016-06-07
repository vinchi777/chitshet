

====Remove local merged branches except master and develop
`git branch --merged | grep -v '^* master$' | grep -v '^  master$' | xargs git branch -d`
