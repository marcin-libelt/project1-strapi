# Strapi application

```
git clone git@github.com:marcin-libelt/project1-strapi.git
```
```
git clone git@github.com:marcin-libelt/project1-gatsby.git
```
npm install gatsby -g
npm install strapi -g

nvm use lts/* ( jedno albo drugie potrzebuje wersji LTS )

npm install ( dla obu )

najpierw odpalić: strapi develop ( kolejność jest istotna )

odpal localhost:1337 i utworz konto w Strapi
 
- utwórz użytkownika Users w CollectionTypes ( Confirmed ON ) - role public
- dodaj 1 artykuł w Articles (title, content, image obowiązkowe, bo nie wiem czemu ale gdy nie ma np. obrazka to gatsby sypie błedami )  w ContentTypes Articles i opublikuj

odpal link ‘localhost:1337/articles’ i sprawdz czy masz dostęp, jeśli (prawdopodobnie) nie to:
ustawienia > users & perssmisions plugin” -> roles dla Public ustaw uprawnienia:

- Application > Article [ find ]
- Users-permissions > User [ find ]

Zrestaruj Strapi -> Ctrl + C …. 
```
strapi develop
```
odpal gatsby … 
```
gatsby develop
```

tym sposobem masz lokalnie działające Strapi i gatsby
cel numer 1 to znaleźć sposob na wrzucenie tego na serwer
cel numer 2 to upload obrazków dla celów Strapi
cel numer 3 podpięcie obsługi email ( moze byc wysyłanie emaila ze strony na adres @)
