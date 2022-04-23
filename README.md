# BOT_Discord_Google_Sheets
Trata-se de um BOT que sua principal função é rolar dados para uma partida de RPG, além disso o script está integrado com o Google Sheets para obter os atributos de cada jogador. Assim quando um jogador pelo chat do Discord pede para o Bot rolar um dado para um determinado atributo o bot além de mostrar quando o jogador tirou no dado, ele também é capaz de informar se o jogador passou ou não no teste.

Para montar a ficha nas planilhas do google basta criar uma tabela com a primeira coluna com o nome dos atributos e cada jogador vai deve ter uma coluna individual, como o exemplo a seguir:

<table border = 1>
<tr><td>Perícia</td><td>Jogador1</td><td>Jogador2</td><td>Jogador3</td><td>Jogador4</td></tr>
<tr><td>FORÇA</td><td>40</td><td>65</td><td>40</td><td>80</td></tr>
<tr><td>CONSTITUIÇÃO</td><td>45</td><td>65</td><td>45</td><td>80</td></tr>
<tr><td>TAMANHO</td><td>85</td><td>60</td><td>60</td><td>70</td></tr>
<tr><td>DESTREZA</td><td>45</td><td>50</td><td>55</td><td>55</td></tr>
<tr><td>APARÊNCIA</td><td>80</td><td>45</td><td>70</td><td>30</td></tr>
</table>
  
O código foi escrito no google colab e foi feito os seguintes import de bibliotecas:

import random <br>
import discord <br>
import asyncio <br>
import datetime <br>
import nest_asyncio <br>
nest_asyncio.apply() <br>
from discord.ext import commands <br>
from google.colab import auth <br>
auth.authenticate_user() <br>
import gspread <br>
from oauth2client.client import GoogleCredentials
