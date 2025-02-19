# Fabio-Blockchain

Shembulli i një Blockchain-i të Thjeshtë
Ky është një implementim i thjeshtë i një blockchain në Python, i dizajnuar për të demonstruar konceptet bazë të funksionimit të një blockchain-i, duke përfshirë minimin, krijimin e blloqeve dhe verifikimin e integritetit të zinxhirit.

Karakteristikat:
Klasa Block: Përfaqëson çdo bllok në blockchain, duke përfshirë atribute si indeksi, koha e krijimit (timestamp), transaksionet, hash-i i bllokut të mëparshëm, nonce (përdoret për minimin) dhe vështirësia.
Minimi: Përdor një mekanizëm të thjeshtë Proof of Work për të minuar blloqet, duke kërkuar që hash-i të fillojë me një numër të caktuar zerosh (i përcaktuar nga niveli i vështirësisë).
Klasa Blockchain: Përfaqëson të gjithë blockchain-in, duke mundësuar krijimin e një blloku genesis, shtimin e blloqeve të reja dhe verifikimin e integritetit të zinxhirit.
Proof of Work: Siguron që hash-i i çdo blloku të përmbushë nivelin e vështirësisë duke minuar dhe duke gjetur një hash që fillon me numrin e kërkuar të zerove.
Si Punohet:
Krijohet një bllok genesis kur inicializohet blockchain-i.
Blloqe të reja mund të shtohen duke thirrur funksionin add_block(), ku secili përmban transaksione.
Integriteti i blockchain-it mund të verifikohet me funksionin is_chain_valid(), i cili kontrollon nëse hash-i i çdo blloku dhe lidhja e tij me bllokun e mëparshëm janë të sakta.
