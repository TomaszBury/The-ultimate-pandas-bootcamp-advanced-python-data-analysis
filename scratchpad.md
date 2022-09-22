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

players.loc[players.isna().values].drop_duplicates()

df2.nationality.nunique()

df2 = players.drop(index=[2,10,21], columns='market_value')

players.select_dtypes(np.number).agg(['min','max','mean'])

def random_case(x):

    funcs = [x.str.swapcase, x.str.lower, x.str.title, x.str.upper]
    
    return choice(funcs)()

players.loc[460, [dtype != object for dtype in players.dtypes]]

# at[] and iat[] should be preferred for single value assignment

