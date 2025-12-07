# Upload Release Asset Action

Upload several assets of a release.

## Example usage

````YML
on:
    push:
steps:
    - name: Update release
      uses: nivaes/update-release@develop  
      env:
        GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
      with:
        tag_name: ${{ github.ref_name }}
        files: |
          ./Artifacts/*.{nupkg,snupkg}

````
