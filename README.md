This tools is using for analysis hong kong mark six probability,and it's related with data source import with next number estimation.

--Import Data Source from https://bet.hkjc.com/marksix/
Parameter :
TYPE :
START DATE:
END DATE:
COOKIE:   

DECLARE @paraIn NVARCHAR(MAX)
DECLARE @paraOut NVARCHAR(MAX)
SET @paraIn = '{"TYPE":"IMPORT_DATA","STARTDATE":"20230101","ENDDATE":"20240331","COOKIE":"s_ecid=MCMID%7C74063766126447319302458112420752425831; ASP.NET_SessionId=gwan3sjhxotkprchpkk1v1fr; AMCVS_06AB2C1653DB07AD0A490D4B%40AdobeOrg=1; s_cc=true; isEU=false; ADRUM=s=1708959628001&r=https%3A%2F%2Fbet.hkjc.com%2Fmarksix%2FResults.aspx%3Fhash%3D-1924203627; BotMitigationCookie_9518109003995423458=\"342053001708959991SOXSf5KdwY8rV8vswpn9UVCJGd8=\"; AMCV_06AB2C1653DB07AD0A490D4B%40AdobeOrg=1585540135%7CMCIDTS%7C19779%7CMCMID%7C74063766126447319302458112420752425831%7CMCAAMLH-1709564832%7C3%7CMCAAMB-1709564832%7CRKhpRz8krg2tLO6pguXWp5olkAcUniQYPHaMWWgdJ3xzPWQmdj0y%7CMCOPTOUT-1708967232s%7CNONE%7CMCAID%7CNONE%7CvVersion%7C4.4.0; s_visit=1; gpv_p5=https%3A%2F%2Fbet.hkjc.com%2Fmarksix%2FResults.aspx%3Flang%3Dch; s_sq=hkjcweb-prd%3D%2526c.%2526a.%2526activitymap.%2526page%253Dbet.hkjc.com%25252Fmarksix%25252Fresults.aspx%2526link%253D%2525E6%252590%25259C%2525E5%2525B0%25258B%2526region%253DdrawResultsAll%2526pageIDType%253D1%2526.activitymap%2526.a%2526.c%2526pid%253Dbet.hkjc.com%25252Fmarksix%25252Fresults.aspx%2526pidt%253D1%2526oid%253Dfunction%252528e%252529%25257Bvarr%25253Db.Qa%252528d%25252Ce%25252Ck%25252Ch%252529%25253Ba.conf.ka%252526%252526%252528r.pa%25253Du%252529%25253Breturnb.vh%252528p%25252Cr%25252Cthis%25252Carguments%252529%25257D%2526oidt%253D2%2526ot%253DDIV"}'
EXEC SP_MARKSIX @paraIn, @paraOut OUTPUT
SELECT @paraOut



![image](https://github.com/decoluk/MarkSixAnalysis/assets/5083289/1fce7c5e-3c27-46fa-b381-829d78ab3fe4)
