public string GetAlimentoMaisPreferido(){
			string alimentoMaisPreferido = "";
			int a = 0;
			int b = 0;
			foreach(var salgado in Blocos) {
                if (salgado.AlimentoPreferido == "Salgado")
                {
                     a++;
                }
			}

			foreach(var doce in Blocos) {
                if (doce.AlimentoPreferido == "Doce")
                {
                     b++;
                }
			}
			if(a>b){
				return alimentoMaisPreferido = "salgado";
			}else
			{
				return alimentoMaisPreferido = "doce";
			}

			
		}
