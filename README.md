# NULL
NUlLL FILE
find . -maxdepth 1 -type f -name '*.sql' ! -name 'database_completo.sql' -print | sort | while IFS= read -r f; do
  cat "$f"
  printf '\n\n'
done > database_completo.sql

