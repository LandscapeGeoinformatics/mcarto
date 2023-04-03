# Matemaatiline kartograafia 2023
Antud juhendid toetavad geograafia eriala magistriõppe kursust <b>Matemaatiline kartograafia LOOM.02.007</b> ja keskenduvad Pythoni matemaatilise kartograafia ja visualiseerimise teegi [Cartopy](https://scitools.org.uk/cartopy/docs/latest/) võimalustele.

Esimene juhend annab ülevaate kaardiakna loomisest, erinevate projektsioonide kasutamisest ja lihtsamate kaardielementide (kaardivõrk, tekst) konstrueerimisest:
* https://github.com/holgervirro/mcarto2023/blob/main/Kaardiakna_juhtimine.ipynb

Teine juhend keskendub täiendavate kaardielementide lisamisele, mille hulka kuuluvad nii lisadetailid (punkttähised, tekst ja legend) kui erinevad matemaatilised ja kartograafilised konstruktsioonid (ortodroom jms):
* https://github.com/holgervirro/mcarto2023/blob/main/Kaardielemendid.ipynb

## Ettevalmistus
Juhendite kasutamine eeldab [Anaconda](https://conda.io/en/main/miniconda.html) olemasolu, mis peaks olema arvutiklassi arvutites tagatud. Kes soovib seda seadistada oma arvutis, võib selleks kasutada Alex Kmochi vastavat [juhendit](https://kodu.ut.ee/~kmoch/geopython2020/L0/Installing_Miniconda_GIS.html).

Pärast Anaconda installimist laadi alla ja paki kuhugi kausta lahti käesolev repositoorium koos kõigi failidega.

`Code -> Download ZIP`

![download_zip](https://github.com/holgervirro/mcarto2023/blob/main/img/download_zip.PNG)-->

Seejärel leia ja ava nn Anaconda Prompt. Loo uus Anaconda keskkond, mille Pythoni versioon on 3.6.

`conda create --name mcarto python=3.6`

<img src="https://raw.githubusercontent.com/hvirro/mcarto/main/img/create_env.PNG" height="150">

Järgmine rida aktiveerib äsjaloodud keskkonna.

`activate mcarto`

<img src="https://raw.githubusercontent.com/hvirro/mcarto/main/img/activate_env.PNG" height="150">

Nüüd tuleks installida vajalikud Pythoni teegid (Jupyter ja Cartopy). Mõlema puhul tulevad kaasa ka mitmed muud teegid, sh Cartopy (`conda install cartopy`) puhul [Matplotlib](https://matplotlib.org/), millele see tugineb.

<img src="https://raw.githubusercontent.com/hvirro/mcarto/main/img/conda_install.PNG" height="150">

Järgnevalt määra aktiivseks kaustaks see, kuhu sai eelnevalt lahti pakitud antud GitHubi repositoorium.

`cd C:\Users\Holger\mcarto-main\mcarto-main`

Lõpuks aktiveeri Jupyteri keskkond.

`jupyter lab`

Avaneb brauser, kus klõps failil laiendiga *.ipynb* avab vastava töövihiku, mida saab brauseri aknas kasutama hakata.
