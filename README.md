
# Nepali-English Parallel Dataset

This repository is dedicated to collecting Nepali-English parallel datasets to facilitate machine translation, NLP research, and more.

## Folder Structure

- `/source`: Contains available sources (in PDF, TXT, or link form) from which you can obtain translations to contribute.
- `/dataset`: This folder holds the contributed datasets in `.tsv` format.

## Dataset Format

Datasets must be in TSV format:
```
Nepali Sentence [tab] English Sentence
```
> I have noticed some inconsistency in how `tab` button on keyboard is treated. So, either use `\t` or better use `\u0009` character like in `./data/parijat_shirish_ko_phool.tsv`.

## How to Contribute

You can contribute by:
1. **Providing a translation source** (uploading a relevant document or link in `/source`)
2. **Submitting actual parallel data** in the `/dataset` folder.
3. **Inspecting and organizing existing sources** in the `/source/Unmanaged` folder.

### Contribution Steps

1. **Create a new branch** with a name that indicates the source of your data.
   ```bash
   git checkout -b source-name
   ```
2. **Add your dataset** in TSV format (Nepali followed by English) to the `/dataset` folder.
3. **Describe the dataset** in the `description.md` file located in the root directory (`./description.md`). Include the source of the dataset, the number of sentences, and any other relevant details.
4. **Submit a pull request** with a detailed description of your contribution.

### Example Commands

1. Clone the repo:
   ```bash
   git clone https://github.com/yourusername/your-repo-name.git
   cd your-repo-name
   ```

2. Create a new branch:
   ```bash
   git checkout -b source-name
   ```

3. Add your dataset (ensure it’s in TSV format):
   ```bash
   cp /path/to/your/dataset.tsv ./dataset/
   ```

4. Update the `description.md` to include what you added.

5. Stage your changes:
   ```bash
   git add .
   ```

6. Commit your changes:
   ```bash
   git commit -m "Added dataset from source-name"
   ```

7. Push to your branch:
   ```bash
   git push origin source-name
   ```

8. Create a pull request with a clear description of your contribution.

## License

This dataset is released under the MIT License. Feel free to use and modify it, but please provide appropriate attribution.