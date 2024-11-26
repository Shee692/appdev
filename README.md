# appdev
My first repository

mkdir barcelona-info
cd barcelona-info
git init

echo "# Barcelona" > README.md
echo "A city of history, culture, and football." >> README.md

git add README.md
git commit -m "Initial commit: Add README.md with an introduction"

git remote add origin https://github.com/<username>/barcelona-info.git
git branch -M main
git push -u origin main
git checkout -b barcelona-details

echo "## Key Attractions in Barcelona" >> README.md
echo "- Sagrada Família" >> README.md
echo "- Park Güell" >> README.md
echo "- La Rambla" >> README.md
echo "- Camp Nou" >> README.md
echo "- Barceloneta Beach" >> README.md

git add README.md
git commit -m "Add key attractions in Barcelona to README.md"
gh pr create --title "Add details about Barcelona" --body "Added key attractions to the README file."
