data_url = 'https://gist.githubusercontent.com/sh7ata/56976975b3c67caabb2efd80bb3a8467/raw/f1b7d2abf6770548edafee58ea15be71e2d28aac/Nutrition.csv'

data_url = 'https://andybek.com/pandas-soccer'

df.rename(columns={'wieght':'Weight (kg)'}, index={0:'Pikachu',1:'Andy'}, inplace=True)

df.rename(mapper={'height': 'Height (m)'},axis='columns')

**dfm.replace(to_replace='\sg', value='', regex=True)**

df.dropna(thresh=df.shape[1], axis=1)

players.loc[players.age.le(25)] == players.loc[players.age <= 25]

<  .lt()
<= .le()
>  .gt()
>= .ge()
== .eq()

data_url = 'https://andybek.com/pandas-soccer'

players.reindex(index=index_players, columns=sorted(players.columns))

unwanted_columns = ['name', 'position', 'position_cat']

players.reindex(columns=set(players.columns).difference(unwanted_rows))


unwanted_rows = [1,2,3,4]

players.reindex(index=set(players.index).difference(unwanted_rows))