# Start with a document

Sometimes it's more convenient to use an editor. Version control becomes
simpler, too.

Just add code, as you normally would:

    html_string = """
    <table>
      <thead>
        <tr>
          <th>Programming Language</th>
          <th>Creator</th>
          <th>Year</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>C</td>
          <td>Dennis Ritchie</td>
          <td>1972</td>
        </tr>
        <tr>
          <td>Python</td>
          <td>Guido Van Rossum</td>
          <td>1989</td>
        </tr>
        <tr>
          <td>Ruby</td>
          <td>Yukihiro Matsumoto</td>
          <td>1995</td>
        </tr>
      </tbody>
    </table>
    """

Additional media.

![](panda-3811734_960_720.jpg)

The start the machine.

    import pandas as pd
    df = pd.read_html(html_string)[0]

So what about the output cell?

    df

You can edit convert the notebook back with `$ notedown input.ipynb --to
markdown --strip > output.md`.

