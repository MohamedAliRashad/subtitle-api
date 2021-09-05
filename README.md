# Browse and Download from subscene.com with just a few lines of python code !

SubtitleAPI is a python package that provide direct access to subtitle content using scraping techniques! You can search for any subtitle you want , also add query filters to your search to remove unwanted content!
## Intsall SubtitleAPI using pip
```
pip install SubtitleAPI
```
Get Movie Subtitles:
```
from subtitleAPI import SubtitleAPI

subscene = SubtitleAPI('english','farsi/persian') # pass languages you want to have in results

subscene.movie(title='Tenet',year=2020,release_type='bluray')
subscene.download()
```
# search IMdB ID
```
subscene.movie(imdb_id='6723592',release_type='bluray')
```
# search for TV Shows

```

subscene.tvshow(title='Game of Thrones',release_type='bluray',season=2,episode=3)

# or

subscene.tvshow(imdb_id='0944947',release_type='bluray',season=2,episode=3)

```
# export zip files After download is Finished !
this method extract all zip files.
```
subscene.download().extract()

```
