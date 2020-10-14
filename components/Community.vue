<template>
  <section class="community">
    <header>
      <h1>1.163 Postings</h1>
      <h2>Jeder User hat das Recht auf freie Meinungsäußerung.</h2>
    </header>
    <div>
      <h3>Welche Postings sind ein Mehrwert für die Community?</h3>
      <div class="postings">
        <posting v-for="item in items" :key="item.headline" :headline="item.headline" :message="item.message"/>
        <div class="success">
          <p>Vielen Dank für deine Auswahl.</p>
          <nuxt-link to="/">Weiter zum Artikel XY</nuxt-link>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data () {
    return {
      items: [
        {
          message: 'Es gab definitiv keine Unterwerfung der Grünen auf Bundesebene. Sowohl Regierungvereinbarung als auch Regierungspraxis sind mit türkis-blau überhaupt nicht zu vergleichen und können sich auch im Vergleich zu rot-schwarzen Vorgängerregierungen durchaus sehen lassen. Dass sie der deutlich kleinere Partner sind macht es selbstverständlich nicht einfacher und umso beachtlicher im Vergleich zu Regierungen in denen die SP sogar den Kanzler stellte. Ein Innenpolitik Redakteur kann das nicht übersehen. Darum wiegt es für mich umso schwerer wenn hier absichtlich und höchst tendenziös vereinfacht wird.'
        },
        {
          message: 'Umwelt betrifft am Ende jeden. Im Normal würde diese ja gar keine Lobby brauchen, wenn man erkennt, das man selbst daran hängt. Bei der Wirtschaft war es aber eben anders gemeint. Wirtschaftstreibende, also da auch die Unternehmer gemeint, sehen sich bei einer roten Regierung wohl nicht in erster Linie vertreten, im Sinne der Interessen. In einem Sozialstaat und hier speziell in einer solchen geführten Stadt, wird es da sicher gerne gesehen, auch eine Adresse zu haben, die in der Gestaltung aktiv beteiligt ist. Und auch da gilt interessanterweise das gleiche wie beim Klima - jeder hängt da drinn, aber dieser Kuchen steht immer in der Diskussion der Teilung oder besser gesagt der Verteilung. Und es geht nicht um Egos, sondern Ideen.'
        },
        {
          headline: 'ob lieb oder nicht lieb:',
          message: 'die GRÜNEN Ur-Anliegen werden uns demnächst wichtig werden. Der nächste warme Sommer kommt bestimmt, der übernächste Skiurlaub ist fraglich, die Kommunikation mit denen, die GRÜN wählen, da fehlt den anderen Parteien etwas an der grünen Grundeinstellung. Grün bedeutet "immer mit Rücksicht auf die Umwelt. Als zweiten Ansatz sehe ich beiden Wiener Grünen die Randgruppen: Schwimmbecken am Gürtel war ja nicht für die ach so urbanen Städer, das sollte ja etwas für die sein, die sonst nur radikale Parteien wählen, weil sie sonst nicht gehört und berücksichtigt werden. So sehr ich auch Ansätze der PINKEN schätze, insbesonders die zur totalen Transparenz, "zuerst die Umwelt und die Ausgegrenzten", das ist eindeutig GRÜN.'
        },
        {
          message: 'Irgendwie kommen mir die Kommentare zum Verhältnis der Roten und Grünen in Wien immer völlig überdramatisiert vor. Ich sehe einfach nicht wo genau die Grünen hier so eine Belastung für die SPÖ sein sollen? Wegen dem bissl Streit im Verkehrsbereich? Der noch dazu stark vom Wahlkampf befeuert wurde und zu dem Ludwig schon selbst quasi gesagt hat, dass es daran nicht scheitern wird? Die Grünen sind doch eh leicht zufrieden zu stellen. Die Neos wären mindestens genauso lästig und mit den Türkisen kann man es sowieso vergessen.'
        },
        {
          headline: 'Ich habe als eigentlicher Grün Wähler kein Problem mit den Grünen.',
          message: 'Aber ich habe eins mit Hebein. Deswegen war es dieses Mal auch rot. Was ich gesehen habe war, speziell, was Radwege angeht: Aktionismus statt Nachhaltigkeit, Show statt visionärer Konzepte und, was die Politik auf Landesebene in Wien angeht und somit meine Wahlentscheidung nachhaltig beeinflusst hat, die mit Abstand schwächste Spitzenkandidatin seit langem. Aktionen zu setzen ist gut und wichtig, aber sorry - ohne Nachhaltigkeit ist Aktionismus reiner Aktionismus und kontraproduktiv.'
        },
        {
          headline: 'Was soll das denn bitte?',
          message: 'Hat man so eine Schlagzeile schon einmal gelesen, als die Grünen in der Bundespartei umgefallen sind. Mir geht dieser doppelte Standard schön langsam sehr auf die Nerven: Während das Verhältnis ÖVP-Grüne hinsichtlich von Dominanz und Unterwerfung quasi naturalisiert wird, so kann Hebein in Bezug auf die SPÖ unterhinterfragt verkünden, dass sie in der Wiener Stadtregierung die "treibende Kraft" sei. Da sollte sich der Standard schon einmal fragen, warum man so eine überzogene Aussage nicht weiter kommentiert.'
        },
        {
          headline: 'SYSTEMWANDEL JETZT ~~~ \o/ ~~~',
          message: 'Im Sinne einer konstruktiven, zügigen Herangehensweise an die großen Herausforderungen der Gegenwart - Gemeinwohl - politische/ökologische Bildung - Arten-/Natur- und Umweltschutz - höhere Mindestlöhne, Senkung der Normal-AZ, - Ökosteuerreform - Fairer Handel, Biolandbau, Ausbau ÖPNV, - massiv höhere Dotation für F & E - Energiesparen und kontinuierliche Reduktion von Fossilenergieverwendung ist mit der blauen und türkisen FPÖ kein Staat zu machen. Letztere bremste auch 30 Jahre lang die SPÖ nun die Grünen. Insofern muss das Ziel sein, durch Argumente Regierungen ohne ÖVP/FPÖ aus Grün/Rot + Partnern zu schaffen und Beweisvernichtung/Aussageverweigung in UAs/vor Gerichten von Blau/Türkis nicht mehr zu tolerieren.'
        },
        {
          message: 'Ich fahre auch in Wien viel Auto und bin damit quasi im Fadenkreuz der grünen Verkehrspolitik. Ich wüsste aber nicht, wo für mich wesentliche Verkehrsprojekte "erlebbar" geworden wären. Schon zu Vassilakous Zeiten haben die sich doch auf eine medial hoch gepushte Fußgängerzone binnen 8 Jahren beschränkt. Bei Hebein gab es dann überhaupt nur noch Zirkusveranstaltungen in der Vorwahlzeit und ein paar Wassersprenger in einzelnen Straßen. Selbst von vergleichsweise einfach umsetzbaren Projekten wie dem Busbahnhof sind wir weiterhin Lichtjahre entfernt, sowas wie den S-Bahn Ring oder eine zweite Stammstrecke ist mit Hebein sowieso eine Utopie.'
        },
        {
          headline: 'mensch vs. umweltschutz',
          message: 'rklärt, etwas überspitzt, den aktuellen (marginalen) untschied zwischen rot und grün am besten. rote werden den fokus in und erst recht nach der krise, immer auf den mensch, sprich arbeitnehmer/-schutz, sprich wirtschaft, legen. grüne auf den umweltschutz und klimawandel. klar ist auch, dass es nur ein gesamtpaket von mensch und umwelt geben kann, aber in krisenzeiten muss man sich des öfteren eben entscheiden... coronazeiten und deren folgeschäden, dafür sind die grünen nicht gemacht.'
        },
        {
          headline: 'das ist ein interessantes phänomen',
          message: 'offensichtlich gibt es eine menge wählerInnen, die großen wert auf eine "reine lehre" legen, und nicht ertragen können, wenn in einer koalition dann a) gewisse kernanliegen keine berücksichtigung finden können und b) an sich widerstrebende dinge mitgetragen werden müssen soll sein, diese leute müssen dann halt warten, dass ihre partei mal wo eine alleinregierung bilden kann... so RICHTIG interessant finde ich aber leute die (nur als beispiel) sich aus enttäuschung über eine koalition mit der övp von grün abwenden und dann neos wählen, die von anfang an völlig andere vorstellungen vertreten - oder aus enttäuschung über rot-grün in wien dann zur övp gehen... da müssen andere dinge eine rolle spielen, die nicht ausgesprochen werden...'
        }
      ]
    }
  }
}
</script>

<style lang="scss">
.community {
  header {
    background: var(--cta);
    color: var(--on-cta);
    padding: 8px 15px;

    h1, h2 {
      font-size: 1.3rem;
      font-weight: normal;
      margin: 0;
    }
  }
}

.success {
  background: green;
  padding: 15px;
  text-align: center;
  color: #fff;

  a {
    color: #fff;
  }
}

.posting {
  + .success {
    display: none;
  }
}
</style>
